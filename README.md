# Alunos
Lucas Noel<br>
Lucas Carvalho


# Como fizemos
Primeiramente pensanmos em uma cena e veio a mente basquete e isso nos baseou nossa cena 

# Static Collider
 - Adicionamos colliders a esse componentes que nao possuem rigidbody para simular um chão e paredes onde por ser um static collider ele poderá interagir com  Dynamic Colliders ou Rigidbody Collider, mas não se moverá pois não possui um rigidbody.
![image](https://github.com/lucasnoelgb/Unity/assets/129121307/622f951f-8a19-4fa1-bade-ec888844df7e)



# Rigidbody Collider
- Este é o collider que possui um "rigidbody" com a opção "IsKinematic" desativada. E na nossa cena foi ultilizados nesses elementos. 
![image](https://github.com/lucasnoelgb/Unity/assets/129121307/63cff668-be14-4006-bbd8-8dcdd82ef6b1)


# Kinematic Collider
 - Este Collider possui um Rigidbody com a opção "IsKinematic" ativada. Eles se comportam de forma semelhante aos Static Colliders, mas podem ser movidos ou ativados ocasionalmente. Na cena ultilizamos ele nessa bola.

 ![image](https://github.com/lucasnoelgb/Unity/assets/129121307/d902c87a-f07d-40ce-8005-922d6732bd20)


# Rigidbody Trigger
- Um rigidbody trigger e uma junção do rigidbody com a opção de trigger. Onde quando esse cubo se encontra com o outro objeto com a tag "Player" que está invisivel o cubo de ato destroi

![image](https://github.com/lucasnoelgb/Unity/assets/129121307/cee4ed6e-1cb3-4891-b75c-459d69990f3d)


# Static Trigger 
- Este tipo de Collider é usado para detectar quando algo entra em sua área sem causar movimento ou colisões físicas. Na cena foi posto em um cubo invisivel e na bola de volei onde ambos ficaram se repelindo

![image](https://github.com/lucasnoelgb/Unity/assets/129121307/6513eca9-8ef6-4018-9296-a45918ef9398)

# Kinematic Rigidbody Trigger 
- Passando pelo objeto com a bola de basquete que tem um script de movimentação esse objeto será coletado e aparecerá uma mensagem logo depois da coleta 

![image](https://github.com/lucasnoelgb/Unity/assets/129121307/2171d9dc-1287-480c-a11b-934e836da1ea)
![image](https://github.com/lucasnoelgb/Unity/assets/129121307/cb9922d5-01b7-4a3c-a8b2-2c7de137610d)

# Codigos
![a](https://github.com/lucasnoelgb/Unity/assets/129121307/817070b1-16eb-4444-9ac8-00b7f481b1ca)
![b](https://github.com/lucasnoelgb/Unity/assets/129121307/e821bc6a-ac86-4c52-841f-eeee25e1f9e1)
![c](https://github.com/lucasnoelgb/Unity/assets/129121307/2697276e-6454-487c-8f4e-9c90b2d833f2)

## movimentacao
![Captura de tela 2023-10-30 115528](https://github.com/lucasnoelgb/Unity/assets/129121307/5af77977-c7ea-4b11-985a-3d65c06bbcba)


## GamePlay



https://github.com/lucasnoelgb/Unity/assets/129121307/cd6e40ee-87e2-4e9f-9fd1-c1efccac07dd










  
  
