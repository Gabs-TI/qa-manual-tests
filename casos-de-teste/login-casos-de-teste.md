# Casos de Teste - Tela de Login

Sistema em teste: [Practice Test Automation](https://practicetestautomation.com/practice-test-login/)

---

## CT001 - Login com credenciais válidas

- **Objetivo**: Verificar se o sistema permite login com dados corretos
- **Pré-requisitos**: Usuário válido cadastrado
- **Passos**:
  1. Acessar a página de login
  2. Preencher o campo de username com `student`
  3. Preencher o campo de password com `Password123`
  4. Clicar no botão "Submit"
- **Resultado Esperado**: Usuário é redirecionado para a página de perfil com a mensagem “Logged In Successfully”

---

## CT002 - Login com senha inválida

- **Objetivo**: Verificar se o sistema exibe mensagem de erro ao usar senha incorreta
- **Pré-requisitos**: Usuário válido cadastrado
- **Passos**:
  1. Acessar a página de login
  2. Preencher o campo de username com `student`
  3. Preencher o campo de password com `senhaerrada`
  4. Clicar no botão "Submit"
- **Resultado Esperado**: Mensagem de erro “Your password is invalid!” deve ser exibida

---

## CT003 - Login com usuário inexistente

- **Objetivo**: Validar comportamento ao tentar logar com usuário que não existe
- **Pré-requisitos**: Nenhum
- **Passos**:
  1. Acessar a página de login
  2. Preencher o campo de username com `naoexiste`
  3. Preencher o campo de password com `Password123`
  4. Clicar no botão "Submit"
- **Resultado Esperado**: Mensagem de erro “Your username is invalid!” deve ser exibida

---

## CT004 - Campos obrigatórios em branco

- **Objetivo**: Garantir que os campos obrigatórios sejam validados
- **Pré-requisitos**: Nenhum
- **Passos**:
  1. Acessar a página de login
  2. Deixar os campos de username e password em branco
  3. Clicar no botão "Submit"
- **Resultado Esperado**: Campos obrigatórios devem ser destacados com mensagem de erro
