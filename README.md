# Raycast
### Dupla: Davi dos Santos e Leonardo Macedo
Atividade solicitada em aula com o intuito de estudarmos a função "Raycast"

## Sobre o Jogo:
![image](https://github.com/Leo-Macedo/Projeto-Raycast-Monstro/assets/127630556/b108002c-0e83-419e-9134-d5072066c566)


Dentro do jogo entramos no papel de um personagem que tem como objetivo procurar e colhetar os papéis que estão espalhados pelo mapa para fugir de uma terrível criatura que nos persegue durante a jogatina, e para que você consiga escapar, devemos colhetar 7 papéis.

## Construção do Jogo:
![CLIQUE (5)](https://github.com/Leo-Macedo/Projeto-Raycast-Monstro/assets/127630556/ca2a40ed-c4d6-4a33-8399-e76b3ab9f0f2)
Começamos criando o cenário com assets da loja, as árvores, pedras, troncos. Adicionamos um SkyBox para fazer a noite estrelada para ficar mais 'sombrio'. Colocamos uma trilha sonora de fundo. Criamos o prefab do papel com um plano e adicionamos uma textura de papel nele para espalharmos pelas árvores. Para o HUD usamos TextMeshPro's e imagens.

## Personagem:
![CLIQUE (7)](https://github.com/Leo-Macedo/Projeto-Raycast-Monstro/assets/127630556/0ac89d8b-4f7b-45f4-b126-2a5ef898f35c)
Como a perspectiva do jogo é em primeira pessoa, nos criamos apenas uma capsula, adicionamos duas mãos e uma lantera na mão esquerda com um spotlight para iluminar. Ele é acompanhado de um script simples apenas para movimentação, rotação e pulo.

## Monstro:
![CLIQUE (9)](https://github.com/Leo-Macedo/Projeto-Raycast-Monstro/assets/127630556/6fa9d540-f599-4dc3-ad9f-b44d5728e9dd)
O monstro é um asset da loja. Colocamos o componente 'Nav Mesh Agent' juntamente ao script (onde decidimos a ditância minima que ele fica do personagem e uma variável para atribuir o personagem, com isso faz que o objeto seguido seja ele) para que ele siga o personagem. Também usamos o 'NavMeshSurface' para delimitar a área que ele pode entrar.

## Códigos:
![CLIQUE (4)](https://github.com/Leo-Macedo/Projeto-Raycast-Monstro/assets/127630556/589ddb95-a95d-499b-a71c-4fbafd45099d)

### Raycast
Utilizamos da função "Raycast" para poder identificar o Prefab dos papéis e, quando o jogador clicasse no lado esquerdo do mouse o "Destroy" executaria sua função:
### Destroy
Dentro da função "Destroy" fizemos com que quando o jogador coletasse o papel, ele iria sumir e seria contabilizado no canto superior esquerdo da tela para que o jogador fique ciente de quantos papéis ele tem para que possa assim ganhar o jogo:
### Prefab
Já na função "Prefab", toda vez que o "Raycast" idêntificasse os papéis, iria aparecer uma pequena mensagem indicando ao jogador o que apertar para poder colhetar os papéis:

![image](https://github.com/Leo-Macedo/Projeto-Raycast-Monstro/assets/127630556/7d57d5a1-9c1e-41a2-b08d-1010e234c817)

### Outras Funções
Também nesse script fizemos um simples sistema para a imagem do 'corra' aparecer por 7 segundos ao iniciar, travar o cursor no centro da tela e quando a contagem de papel chegar a 7 ativa a tela de final do jogo e também libera o cursor.

# GamePlay do Jogo (ligue o som para experiência completa)


https://github.com/Leo-Macedo/Projeto-Raycast-Monstro/assets/127630556/70a51e15-61af-42a7-97f0-4bd7fb4a30a5







