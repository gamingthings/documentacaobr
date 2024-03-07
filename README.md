![image](https://github.com/gamingthings/documentacaobr/assets/162502847/6cabb898-d84b-4c5b-9adf-b80c089b3840)![image](https://github.com/gamingthings/documentacaobr/assets/162502847/cefcb778-c3d9-4469-b752-57864ec591f5) 
###  AVISO
Eu não usaria este docs se você pretende seguir a area de t.i ou correlacionados , pois o inglês e este assunto é nescessario/conhecimento basico ou essencial para o mercado de trabalho. CASO MUDE DE IDEIA use o docs da pagar.me https://docs.pagar.me/
`1-   passo você ira entrar no github do bento quirino na aba aos , você vai precisar do insomnia e do arquivo json encontrado no repo `https://github.com/Bento-Quirino/AOS/blob/main/insomnia-simulado.json
`2- você vai abrir o insomnia e vai clicar nas seguintes instruções : ![image](https://github.com/gamingthings/documentacaobr/assets/162502847/6745cbe7-46a0-494f-8b36-b5375ec951d3)

`create/criar - import/importar - choose a file/escolha um arquivo ![image](https://github.com/gamingthings/documentacaobr/assets/162502847/178f12ce-8b65-4435-a70a-c0b93cc26049)

3- honestamente não sei se esta parte está 100% correta, mas deu certo pra mim : troque o api_key por base url e depois disso vocês vão notar que não possuem autorização , no 4 ensinarei como .
![image](https://github.com/gamingthings/documentacaobr/assets/162502847/7a002613-4a0a-4325-96dc-3471d68d3d2c)

![image](https://github.com/gamingthings/documentacaobr/assets/162502847/00998545-28c2-4832-9a53-0d7ec0cb48ee)

4- no header vocês iram escrever Authorization e do outro lado coloque api em seguida clique cntrl espaço e você terá um markdown roxo igual o da imagem coloque ele ![image](https://github.com/gamingthings/documentacaobr/assets/162502847/bb5d3e5c-1c5b-4c3f-92c6-17ff5b1c3ed1)

5- obviamente essa request é invalida até por que ela não tem um body eu não estou enviando nada para api com este post ![image](https://github.com/gamingthings/documentacaobr/assets/162502847/c61e9cb0-5347-4e16-9f9a-1a5e74876c7a) crie um arquivo json  ao lado de parameters  e insira este codigo 
{
  "birthdate": "xx/xx/xxxx",
  "name": "",
  "email": "",
  "gender": "" 

}
nome é obrigatorio email tem que ser unico , gender só pode ser male ou female! o birthdate é dia mes ano
## TROQUE OS NOMES PADRÃO CODIGOS DATA DE NASCIMENTO ETC!!! 
Pronto seu usúario foi criado
se quiser listar eles é só usar a aba de baixo list user pagination , exclua o code/codigo que tem em baixo do size e coloque o valor 1 e 10 ![image](https://github.com/gamingthings/documentacaobr/assets/162502847/96fa207c-0331-4487-ab2e-6415277e9bad) se não ele vai puxar um arquivo especifico com codigo especifico como todos os codigos na vdd são gerados! então  apague para listar todos sem execesão ou deixe mas veja qual seu codigo na parte que cria o usuario em preview ou vc vai ter um codigo ou id de usuario

6-  para criar o pedido você vai precisar do id do seu usuario ![image](https://github.com/gamingthings/documentacaobr/assets/162502847/9ebcc614-3e1f-4a40-a571-9428f7370f9c)

7- criando o pedido duplique este request 
![image](https://github.com/gamingthings/documentacaobr/assets/162502847/96585822-8229-4c1e-b120-789877443020)
muda para post 
![image](https://github.com/gamingthings/documentacaobr/assets/162502847/c5cc652d-19c2-4e04-8536-6687e4487eab)
![image](https://github.com/gamingthings/documentacaobr/assets/162502847/0458a346-513c-4647-b129-fb0c06979897)
como nos outros passos abra o json e faça um codigo 
## MUDE OS VALORES TODOS!!!
codigo do body/json será este, note que o id é do usuario que criamos anteriormente altere este id para o do seu usuario:  
  "customer_id": "cus_ZxVWkKF9DT0vWG65",    
  "items": [
    {
      "amount": 1,
      "description": "objetocomprado",
      "quantity": 927,
      "code": "xxxxx01"
    }
  ],
  "payments": [
    {
      "cash": {
        "cash": "2000"
      },
      "payment_method": "cash"
    }
  ]
}

para listar apenas use o request http acima  vulgo listar pedidos
e para obter escreva destá forma em parametros   ![image](https://github.com/gamingthings/documentacaobr/assets/162502847/dde3a8ab-5481-47c4-9485-78df89ea0563) note que quando listar sua compra/pedido irá aparecer um id do pedido!o order_id precisa ser isso sobre documentação  ![image](https://github.com/gamingthings/documentacaobr/assets/162502847/92620eb5-35ef-40f6-befa-19a34e9b62f3) aqui é onde fica o segredo é usar ## para criar o titulo ou textos destacados usar `
este simbolo para enquadrar coisas importantes
sempre coloque em seus docs seu body/json e sua base url https://api.pagar.me/core/v5
seu endpoint que pode ser /costumers ,/orders etc 








## NÃO MANDEM CEBOLA PRA MINHA CASA!


