# Desafio de Programação

## Introdução

Deseja-se desenvolver um projeto que simula um feed simples de uma rede social. Ele consiste de dois objetivos e os detalhes de cada objetivo é dado a seguir.

## A Rede Social

O primeiro objetivo deste desafio é desenvolver uma aplicação web que simula uma rede social. Você é responsável por implementar as páginas, componentes e estilos.

Esta rede social precisa prover:
- Feed de posts:
  - É possível criar, editar e deletar um post;
  - Listar posts (título e conteúdo) em uma lista;
  - Mostrar usuários em um grid ou lista;
- Detalhes de posts com comentários:
  - Mostrar comentários em uma lista;
- Detalhes de usuários:
  - Mostrar os posts dos usuários;
  - Mostrar os álbuns dos usuários;
- Detalhes do álbum de usuário:
  - Grid com fotos do álbum;

## Recuperando e Atualizando os Dados

O segundo objetivo deste desafio é recuperar os dados da rede social do serviço [JSON Placeholder](https://jsonplaceholder.typicode.com/guide/). Você é responsável por recuperar dados relacionados a posts, comentários, usuários e álbuns usando a API do **JSON Placeholder**.

**JSON Placeholder** provê dados que simulam:
- 10 usuários
- 100 posts
- 500 comentários
- 100 álbuns
- 5000 ftos

**IMPORTANTE❗: Os dados no JSON Placeholder são imutáveis. Os endpoints que modificam dados nunca atualizam os dados originais.**

### Endpoints

Aqui você pode encontrar todos os endpoints disponíveis para serem usados neste desafio.

Formato: `MÉTODO HTTP` descrição do endpoint

#### Usuário

- `GET` recuperar todos os usuários:
```
https://jsonplaceholder.typicode.com/users
```
- `GET` recuperar um único usuário:
```
https://jsonplaceholder.typicode.com/users/<USER-ID>
```
- `GET` recuperar posts de um usuário:
```
https://jsonplaceholder.typicode.com/posts/<USER-ID>

```

#### Álbum
- `GET` recuperar álbuns de um usuário:
```
https://jsonplaceholder.typicode.com/albums/<USER-ID>
```
- `GET` recuperar fotos de um álbum:
```
https://jsonplaceholder.typicode.com/albums/<USER-ID>/photos
```

#### Posts

- `GET` recuperar todos os posts:
```
https://jsonplaceholder.typicode.com/posts
```

- `GET` recuperar um único post:
```
https://jsonplaceholder.typicode.com/posts/<POST-ID>
```
- `GET` recuperar comentários de um post:
```
https://jsonplaceholder.typicode.com/posts/<POST-ID>/comments
```
- `POST` criar um post:
```
https://jsonplaceholder.typicode.com/posts
```
- `PUT` atualizar um post:
```
https://jsonplaceholder.typicode.com/posts/<POST-ID>/
```
- `PATCH` atualizar um post:
```
https://jsonplaceholder.typicode.com/posts/<POST-ID>/
```

- `DELETE` deletar um post:
```
https://jsonplaceholder.typicode.com/posts/<POST-ID>/
```

### Feedback para o usuário

Você precisa mostrar ao usuário se um request para a API completou corretamente (`POST`, `PUT`, `PATCH`,`DELETE`) ou não (qualquer método HTTP). Você pode mostrar isso através de diálogos, toasts ou notificações.
