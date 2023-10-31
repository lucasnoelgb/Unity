# Alunos
Lucas Noel<br>
Lucas Carvalho


# Como fizemos
Primeiramente pensanmos em uma cena e veio a mente basquete e isso nos baseou nossa cena. 

# Static Collider
 - Adicionamos colliders a esse componentes que nao possuem rigidbody para simular um chão e paredes onde por ser um static collider ele poderá interagir com  Dynamic Colliders ou Rigidbody Collider, mas não se moverá pois não possui um rigidbody.
  
![image](https://github.com/lucasnoelgb/Unity/assets/129121307/2b8febf7-7f95-4307-b9b6-1474eea1793c)



# Rigidbody Collider
- Este é o collider que possui um "rigidbody" com a opção "IsKinematic" desativada. E na nossa cena foi ultilizados nesses elementos.
 
![image](https://github.com/lucasnoelgb/Unity/assets/129121307/914e709d-290e-48dd-8658-95bf94413525)


# Kinematic Collider
 - Este Collider possui um Rigidbody com a opção "IsKinematic" ativada. Eles se comportam de forma semelhante aos Static Colliders, mas podem ser movidos ou ativados ocasionalmente. Na cena ultilizamos ele nessa bola.

 ![image](https://github.com/lucasnoelgb/Unity/assets/129121307/d902c87a-f07d-40ce-8005-922d6732bd20)


# Rigidbody Trigger
- Um rigidbody trigger e uma junção do rigidbody com a opção de trigger. Onde quando esse cubo se encontra com o outro objeto com a tag "Transparente" que está invisivel o cubo de ato destroi.

![image](https://github.com/lucasnoelgb/Unity/assets/129121307/cee4ed6e-1cb3-4891-b75c-459d69990f3d)


# Static Trigger 
- Este tipo de Collider é usado para detectar quando algo entra em sua área sem causar movimento ou colisões físicas. Na cena foi posto em um cubo invisivel e na bola de volei onde ambos ficaram se repelindo

![image](https://github.com/lucasnoelgb/Unity/assets/129121307/6513eca9-8ef6-4018-9296-a45918ef9398)

# Kinematic Rigidbody Trigger 
- Passando pelo objeto com a bola de basquete que tem um script de movimentação, esse objeto será coletado e aparecerá uma mensagem logo depois dele ser pego. 

![image](https://github.com/lucasnoelgb/Unity/assets/129121307/2171d9dc-1287-480c-a11b-934e836da1ea)
![image](https://github.com/lucasnoelgb/Unity/assets/129121307/f19ffd66-c192-47ec-9478-e8efe7bf8c3d)


# Codigos 


## Static Trigger
    using System.Collections;
    using System.Collections.Generic;
    using UnityEngine;


    public class LaunchObject : MonoBehaviour 
       {
    public float launchForce = 10f;

    private void OnTriggerEnter(Collider other)

    {
        Rigidbody rb = other.GetComponent<Rigidbody>();

        if (rb != null)
        {

            rb.AddForce(Vector3.up * launchForce, ForceMode.Impulse);

              }
 

          }


      }
 

## Rigidbody Trigger
     using System.Collections;
     using System.Collections.Generic;
     using UnityEngine;

     public class ri : MonoBehaviour
     {

         private void OnTriggerEnter(Collider other)
      {
            if (other.CompareTag("Transparente"))
          {
                Destroy(gameObject);

          }

      }  
    }   


## Kinematic Collider 
    using System.Collections;
    using System.Collections.Generic;
    using UnityEngine;

       public class ObjetoKinematic: MonoBehaviour
         {
       private void OnTriggerEnter(Collider other)
        {

            if (other.CompareTag("quadrado"))
        {
            AtivarEventoPegar();
        }
            }

    
          private void AtivarEventoPegar()
        {


         Debug.Log("Objeto coletado! ");
         gameObject.SetActive(false);
              }
 
         }
## movimentação
    using System.Collections;
    using System.Collections.Generic;
    using UnityEngine;

    public class Mo : MonoBehaviour
    {
       //movimento
    public float fast = 1f;

    void Start()

    { 
    }

    void Update()
    {
        //movimento
       
        if (Input.GetKey(KeyCode.S))
        {
            transform.Translate(0f, 0f, -fast);
        }
      
        
    }
    }


## GamePlay



https://github.com/lucasnoelgb/Unity/assets/129121307/cd6e40ee-87e2-4e9f-9fd1-c1efccac07dd










  
  
