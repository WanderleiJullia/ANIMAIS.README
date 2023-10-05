# ANIMAIS.README
A lista a seguir,  corresponde as atividades complementares 2. 

Atividade a seguir, tem o objetivo de executar uma lista de comandos referente a lista de animais. Conforme orientação de cada código, terá imagens e a explicação dos comandos utilizados.

![01](https://github.com/WanderleiJullia/ANIMAIS.README/assets/144744092/02cade92-5a13-48da-9716-71ca5275729e)

# Alteração de Nome. 
    update Animais set nome = 'Goofy' where id = 15; 

   ![02](https://github.com/WanderleiJullia/ANIMAIS.README/assets/144744092/fc02017e-cdba-4000-941a-d17ba5da2b88)


º Para uma alteração de nome em uma tabela, precisamos utilizar WHERE, para assim selelcionar a linha ou a coluna que queremos a mudança. Caso ao contrario, todos os itens da tabela terá alteração. 


# Alteração de Peso. 

    update Animais set peso = '10' where id = 4;

![03](https://github.com/WanderleiJullia/ANIMAIS.README/assets/144744092/9a99cefa-dd62-40d4-a042-710e912bb1df)

º Solicitação de mudança de peso do ID 04, de 201Kg para 10.00kg. 

# Alteração de Cor. 

    update Animais set cor = 'Laranja' where id (1, 3, 7, 12, 13, 15, 17, 22, 25);

º Solicitação de Mudança de cor somente da especie dos Gatos. Com isso, o WHERE, teve o objetivo de especificar cada ID que seria necessario ser feita alteração. 

# Criação de uma nova Tabela. 

    alter table Animais add Altura decimal(10,2); 

  ![04](https://github.com/WanderleiJullia/ANIMAIS.README/assets/144744092/8f31e5ab-97a8-4e78-a3d5-2472e130a44d)


   º Criação de uma nova coluna na tabela dos Animais.    

# Campo Observação. 

    alter table Animais add Observações varchar(50); 
    
![05](https://github.com/WanderleiJullia/ANIMAIS.README/assets/144744092/ac3db4b3-3bcf-4393-8345-7071540b17f1)

º Coluna inserida na tabela de Animais, referente a um campo de obserações. 

# Remover animais. 

    delete from Animais where peso > 200;

 ![06](https://github.com/WanderleiJullia/ANIMAIS.README/assets/144744092/5fd17679-3dff-4911-a507-aa4ed194affd)

 º Comando solicitado para remover todos os animais da lista que possui o peso maior que 200kg.

 º Para esse comando ser realizado na plataforma MySQL, precisamos utilizar o seguinte código, para assim desabilitar a função de segurança. Com a função desabilitada, podemos remover todos os comandos na Tabela. 

     SET SQL_SAFE_UPDATES = 0;


# Remover animais (C) 

    delete from Animais where nome like '%c' ; 

  ![07](https://github.com/WanderleiJullia/ANIMAIS.README/assets/144744092/183b2146-00e7-4c37-8904-dbfe1f6b47ac)

  º Realizando a remoção de todos os animais que possui a inicial C. 

  # Remover cor 

      alter table Animais drop cor;

  ![08](https://github.com/WanderleiJullia/ANIMAIS.README/assets/144744092/71a83436-001d-469b-a6f1-a9266e051d3d)

º Para essa função, deletamos a coluna cor por completa. 

# Remover Gatos e Cachorros 

    delete from Animais where especie in ('Gato', 'Cachorro');

 ![09](https://github.com/WanderleiJullia/ANIMAIS.README/assets/144744092/5be29883-1771-4845-835e-9f95f4f9e09b)

 º Realizando a remoção dos animais Gato e Cachorro, sobrou somente os animais na lista acima. 

 # Remover Data de Nascimento. 

     alter table Animais drop nasc; 

  ![09](https://github.com/WanderleiJullia/ANIMAIS.README/assets/144744092/3115452c-8c2e-4acd-a88e-ff0987fc7cb8)

  º Utilizando a mesma imagem, para identificar a remoção das datas e nacimentos  dos animais. 

  # Remover Animais/ Especies. 

      drop table Animais; 
    
      drop table especies; 

 º Conforme solicitado, realizando a remoção das colunas acima, acabamos de finalizar nossa tabela. 

 


Jullia Santos Wanderlei 

Bancos de Dados. 



