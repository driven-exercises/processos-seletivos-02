# 🌎 Descrição

- Seja bem-vindo(a) ao jornal **TopNews**!
- Aqui prezamos muito pelo jornalismo de qualidade e pela velocidade em que a informação chega aos nossos leitores e leitoras. E para conseguir entregar o melhor, precisamos nos apoiar na tecnologia e para isso nós precisamos da sua ajuda!
- Neste desafio, você implementará o back-end de uma aplicação que apoiará a nossa plataforma de notícias rápidas.

# ✅ Requisitos obrigatórios

- Requisitos técnicos
  - Devem ser utilizadas, obrigatoriamente, as tecnologias que já fazem parte da nossa stack tecnológica pra construção do back-end:
    - Node;
    - Express;
    - TypeScript;
    - Prisma (ORM);
    - Postgres;
    - Jest;
    - Supertest.
  - É esperado que o projeto esteja organizado com uma arquitetura em camadas (*Layered Architecture*), com a correta divisão do código na responsabilidade de cada camada. Ou seja: routers, controllers, services, repositories, etc.
  - O projeto deve ter testes automatizados. Projetos sem a cobertura mínima de testes não serão avaliados e o(a) candidato(a) será desclassificado(a).
    - A cobertura mínima deve ser de 70%.
  - O desafio deve ser entregue rodando no ar, hospedado na plataforma de sua preferência! O importante é que possamos ter uma URL em que o projeto possa ser usado/testado.

- Rotas
  - O back-end da aplicação deve possuir as seguintes rotas:
    - **GET** `/news`
      - Este rota deve retornar todas as notícias cadastradas. Caso não exista nenhuma, retornar um array vazio.
    - **GET** `/news/:id`
      - Esta rota deve retornar a notícia com o id específico. Caso não exista nenhuma, retornar o erro 404.
    - **POST** `/news`
      - Esta rota deve cadastrar uma nova notícia.
      - Formato:
          
          ```js
          title: string
          text: string
          author: string
          firstHand: boolean *(opcional)*
          ```
          
      - Se o formato enviado não for compatível, retornar erro 400.
    - **PUT** `/news/:id`
      - Esta rota deve alterar os dados de uma notícia.
      - Formato:
          
          ```js
          title: string
          text: string
          author: string
          firstHand: boolean *(opcional)*
          ```
          
      - Se o id não for encontrado, retornar o erro 404.
      - Se o formato enviado não for compatível, retornar erro 400.
    - **DELETE** `/news/:id`
      - Esta rota deve deletar uma notícia.
      - Se o id não for encontrado, retornar o erro 404.

### 👀 Observações
---

- Nesse desafio iremos avaliar tanto a qualidade da aplicação entregue a nível de funcionalidade quanto a nível de qualidade de código. Esperamos que você dê o seu melhor nesses dois sentidos!
- **O que não estiver descrito explicitamente nesses requisitos espera-se que você tome a decisão por conta própria seguindo bom senso e as boas práticas da comunidade, itens que também estão sendo avaliados.**