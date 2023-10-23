# Tutorial: Criando uma Página HTML Básica para um Currículo

Neste tutorial, vou mostrar a você como criar uma página HTML simples para exibir um currículo. O código HTML que você forneceu é uma estrutura de exemplo que pode ser usada como ponto de partida.

## Pré-requisitos

Antes de começar, certifique-se de ter um editor de texto, como o Visual Studio Code, Sublime Text ou qualquer outro de sua escolha, instalado em seu computador.

### Passo 1: Preparar o Arquivo HTML

Primeiro, você precisa criar um arquivo HTML. Abra seu editor de texto e crie um novo arquivo com a extensão `.html`. Vamos chamá-lo de `curriculo.html`.

### Passo 2: Definir a Estrutura Básica do HTML

Aqui está o código inicial que define a estrutura básica de um documento HTML:

```html
<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Seu Nome - Currículo</title>
</head>
<body>
    <!-- Conteúdo do currículo será adicionado aqui -->
</body>
</html>
```

Neste código:

- `<!DOCTYPE html>` define o tipo de documento como HTML5.
- `<html lang="pt-br">` define o idioma da página como português brasileiro.
- A seção `<head>` contém metadados, como a codificação de caracteres, a viewport e o título da página.
- A seção `<body>` é onde você adicionará o conteúdo do seu currículo.

### Passo 3: Adicionar Informações Pessoais

Agora, você pode adicionar suas informações pessoais, como nome, cidade, telefone e e-mail. Substitua `"Seu Nome"` pelo seu nome e preencha as informações conforme necessário:

```html
<h1>Seu Nome</h1>
<p>Cidade: Sua Cidade</p>
<p>Telefone: Seu Telefone</p>
<p>Email: Seu Email | LinkedIn: <a href="https://linkedin.com/in/seu-linkedin">seu-linkedin</a></p>
```

### Passo 4: Adicionar Seções de Conteúdo

Você pode adicionar seções para "Sobre Mim", "Experiência", "Educação", "Licenças e Certificações" e outras informações relevantes. Aqui está um exemplo de como adicionar a seção "Sobre Mim":

```html
<section>
    <h2>Sobre Mim</h2>
    <p>Texto sobre você e sua carreira.</p>
</section>
```

### Passo 5: Adicionar Imagens

Se você deseja adicionar uma foto ao seu currículo, você pode usar a tag `<img>`. Certifique-se de que a imagem esteja localizada no mesmo diretório que o arquivo HTML ou forneça o caminho correto para a imagem no atributo `src`. Por exemplo:

```html
<div class="profile-picture">
    <img src="./assets/sua-foto.jpg" alt="Sua Foto">
</div>
```

Lembre-se de substituir `"sua-foto.jpg"` pelo nome do arquivo de sua foto.

### Passo 6: Adicionar Seção de Experiência

A seção de experiência é onde você lista suas experiências profissionais. Cada trabalho deve ser listado como um item de lista. Você pode adicionar uma seção de experiência após a seção "Sobre Mim". Aqui está um exemplo de como adicionar um trabalho:

```html
<section>
    <h2>Experiência</h2>
    <ul>
        <li>
            <h3>Nome do Cargo - Nome da Empresa</h3>
            <p>Localização da Empresa</p>
            <p>Data de Início - Data de Término (se aplicável)</p>
            <p>Descrição das responsabilidades e realizações no cargo.</p>
        </li>
        <!-- Repita para cada trabalho -->
    </ul>
</section>
```

### Passo 7: Adicionar Seção de Educação

A seção de educação é onde você lista suas qualificações acadêmicas. Cada instituição e curso deve ser listado como um item de lista. Você pode adicionar uma seção de educação após a seção de experiência. Aqui está um exemplo:

```html
<section>
    <h2>Educação</h2>
    <ul>
        <li>
            <h3>Nome da Instituição</h3>
            <p>Título do Curso, ou Área de Estudo</p>
            <p>Data de Início - Data de Término (se aplicável)</p>
        </li>
        <!-- Repita para cada instituição e curso -->
    </ul>
</section>
```

### Passo 8: Adicionar Seção de Licenças e Certificações

A seção de licenças e certificações é onde você lista suas credenciais e certificações profissionais. Cada certificação deve ser listada como um item de lista. Você pode adicionar uma seção de licenças e certificações após a seção de educação. Aqui está um exemplo:

```html
<section>
    <h2>Licenças e Certificações</h2>
    <ul>
        <li>
            <h3>Nome da Certificação</h3>
            <p>Concedido por: Nome da Instituição</p>
            <p>Data de Concessão</p>
        </li>
        <!-- Repita para cada certificação -->
    </ul>
</section>
```

### Passo 9: Estilizar o Currículo com CSS

Aqui está como o CSS foi estilizado no exemplo do currículo. Você pode personalizar essas regras CSS para atender às suas preferências de estilo. No exemplo abaixo, eu fornecerei uma breve explicação de cada parte do CSS:

```html
<style>
    @page {
        size: A4;
        margin: 20;
    }

    header {
        display: flex;
        align-items: center;
        margin-bottom: 20px;
    }

    .profile-picture {
        width: 120px;
        height: 120px;
        border-radius: 50%;
        overflow: hidden;
        margin-right: 20px;
    }

    .profile-picture img {
        width: 100%;
        height: 100%;
        object-fit: cover;
    }

    .header-info {
        flex: 1;
    }

    .header-info h1 {
        font-size: 24px;
        margin: 0;
    }

    .header-info p {
        margin: 5px 0;
    }

    body {
        font-family: "Montserrat", sans-serif;
        font-size: 12px;
        color: #000;
        background-color: #fff;
        margin: 0;
        padding: 20px;
    }

    section {
        margin-bottom: 20px;
    }

    h2 {
        font-size: 16px;
        margin-bottom: 10px;
    }

    h3 {
        font-size: 14px;
        margin-bottom: 5px;
    }

    p {
        margin: 0;
    }

    ul {
        list-style-type: none;
        padding: 0;
        margin: 0;
    }

    li {
        margin-bottom: 10px;
    }
</style>
```

Neste exemplo de CSS:

- `@page` define o tamanho da página como A4 e as margens da página.
- `.profile-picture` estiliza a foto de perfil, define seu tamanho e aplica um corte arredondado.
- `.header-info` estiliza as informações pessoais na seção de cabeçalho.
- `.body` define a fonte do texto, tamanho da fonte, cor de texto e cor de fundo da página.
- `section`, `h2`, `h3`, `p`, `ul`, e `li` estilizam várias partes do currículo, como as seções, cabeçalhos, parágrafos e listas.

Você pode personalizar as propriedades CSS, como cores, fontes e tamanhos, de acordo com suas preferências. Além disso, você pode adicionar mais regras CSS para estilizar elementos específicos no seu currículo, como links, formatação de texto e cores de fundo.

Certifique-se de que o CSS seja colocado na seção `<style>` dentro da tag `<head>` do seu arquivo HTML ou vincule um arquivo CSS externo, se preferir.

Com isso, você personalizou o estilo do seu currículo em HTML. Lembre-se de salvar o arquivo HTML e o CSS e abri-los em um navegador para ver o resultado final. Continue ajustando o CSS até atingir o visual desejado para o seu currículo.
