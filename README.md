# Plano de Testes - UI Testing

### Casos de teste: Etapa 1 - Login

1. **Login com usuário aleatório**

   **Passos:** Acesse a página e insira um usuário e senha aleatórios.  
   **Resultado obtido:** Ao inserir um usuário aleatório, o mesmo foi barrado.  
   **Resultado esperado:** Ao inserir um usuário aleatório, a plataforma deve barrar a entrada do usuário.  
   **Status:** Passou  
   **Ajuste:** Necessário ajustar o layout do retorno da resposta, o modal está quebrando impossibilitando a visualização do usuário.
   
   ![Sem título](https://github.com/user-attachments/assets/41372df4-5da1-4501-90a7-363258add946)


3. **Login inserindo apenas usuário**

   **Passos:** Acesse a página e insira apenas o seu usuário e clique em "Login".  
   **Resultado obtido:** Ao inserir usuário, a plataforma retornou uma mensagem informando para inserir a senha.  
   **Resultado esperado:** Ao inserir apenas o usuário, a plataforma deve retornar uma mensagem informando que é necessário inserir usuário e senha.  
   **Status:** Passou

4. **Login inserindo apenas senha**

   **Passos:** Acesse a página e insira apenas a sua senha e clique em "Login".  
   **Resultado obtido:** Ao inserir senha, a plataforma retornou uma mensagem informando para inserir usuário e senha.  
   **Resultado esperado:** Ao inserir apenas o usuário, a plataforma deve retornar uma mensagem informando que é necessário inserir usuário e senha.  
   **Status:** Passou

5. **Login com senha inválida**

   **Passos:** Acesse a página e insira seu usuário com uma senha inválida e clique em "Login".  
   **Resultado obtido:** Ao inserir senha inválida, a plataforma retorna o erro, mas a mensagem está em inglês.  
   **Resultado esperado:** A plataforma deve retornar o erro com a mensagem em português.  
   **Ajuste:** Ajustar tradução da mensagem e layout do retorno da resposta, que está vindo quebrado, impossibilitando a visualização do usuário.  
   **Status:** Necessário ajuste

6. **Login com usuário inválido**

   **Passos:** Acesse a página e insira apenas seu usuário inválido e clique em "Login".  
   **Resultado obtido:** Ao inserir o usuário inválido, a plataforma retorna o erro, mas a mensagem está em inglês.  
   **Resultado esperado:** A plataforma deve retornar o erro com a mensagem em português.  
   **Ajuste:** Ajustar tradução da mensagem e layout do retorno da resposta, que está vindo quebrado, impossibilitando a visualização do usuário.  
   **Status:** Necessário ajuste

7. **Limite de caracteres**

   **Passos:** Acesse a página e insira mais que 50 caracteres no usuário e senha.  
   **Resultado obtido:** Campos usuário e senha estão sem limitação de caracteres.  
   **Resultado esperado:** Os campos usuário e senha devem conter limitação de caracteres.  
   **Status:** Necessário ajuste

8. **Teste de Layout clique no ícone "x" para apagar texto completo**

   **Passos:** Insira um usuário e senha incorretos e clique em "Login".  
   **Resultado obtido:** Ao inserir o texto incorreto e clicar em login, é retornado o erro. Ao tentar apagar o texto clicando no ícone "x" do usuário e senha, o mesmo não funciona.  
   **Resultado esperado:** Ao clicar no ícone "x", o texto deve ser apagado.  
   **Status:** Necessário ajuste

### Casos de teste: Etapa 2 - Ordenação e filtragem de produtos

1. **Verificar se os produtos podem ser ordenados de A a Z e de Z a A**

   **Passos:** Ordene o filtro por nome de A a Z e de Z a A.  
   **Resultado obtido:** A filtragem de A a Z e Z a A não está funcionando conforme o esperado.  
   **Resultado esperado:** Ao aplicar o filtro de A a Z e Z a A, a plataforma deve ordenar por ordem alfabética conforme a filtragem aplicada.  
   **Status:** Necessário ajuste

2. **Verificar se os produtos podem ser ordenados por preço (do menor para o maior e vice-versa)**

   **Passos:** Ordene o filtro do menor para o maior e vice-versa.  
   **Resultado obtido:** Ao aplicar o filtro, a plataforma ordenou conforme o esperado.  
   **Resultado esperado:** O filtro deve ser aplicado conforme ordenado pelo usuário.  
   **Status:** Passou

### Casos de teste: Etapa 3 - Visualização do produto

1. **Verificar se é possível clicar e visualizar o produto**

   **Passos:** Clique em algum produto.  
   **Resultado obtido:** Ao clicar no produto, é possível visualizar conforme o esperado.  
   **Resultado esperado:** Ao clicar no produto, o mesmo deve ser aberto e visualizado pelo usuário.  
   **Status:** Passou

2. **Verificar se é possível clicar em "voltar para produtos"**

   **Passos:** Ao clicar para visualizar um produto específico, visualize se é possível clicar no botão "Voltar para produtos" e visualizar a página anterior.  
   **Resultado obtido:** Está sendo possível clicar para retornar aos produtos na página anterior.  
   **Resultado esperado:** Deve ser possível clicar em "Voltar para produtos" para retornar aos produtos da página anterior.  
   **Status:** Passou

### Casos de teste: Etapa 4 - Adicionar e remover do carrinho

1. **Verificar se é possível adicionar o produto ao carrinho**

   **Passos:** Clique na opção "Adicionar ao carrinho" e verifique se está funcional.  
   **Resultado obtido:** Está sendo possível clicar em "Adicionar ao carrinho".  
   **Resultado esperado:** Deve ser possível clicar em "Adicionar ao carrinho".  
   **Status:** Passou

2. **Verificar se é possível navegar até o carrinho clicando no ícone do carrinho**

   **Passos:** Clique no ícone de carrinho.  
   **Resultado obtido:** Está sendo possível clicar no ícone de carrinho e visualizar os produtos adicionados.  
   **Resultado esperado:** Deve ser possível clicar no carrinho.  
   **Status:** Passou

3. **Verificar se é possível editar a quantidade do produto**

   **Passos:** Na visualização do carrinho, verifique se é possível editar a quantidade de produtos.  
   **Resultado obtido:** Não é possível editar a quantidade de produtos.  
   **Resultado esperado:** Deve ser possível editar a quantidade de produtos.  
   **Status:** Necessário ajuste

4. **Verificar se é possível remover o produto do carrinho**

   **Passos:** Na visualização do carrinho, clique em "Remover".  
   **Resultado obtido:** Ao clicar em "Remover", o produto está sendo removido do carrinho.  
   **Resultado esperado:** Ao clicar em "Remover", o produto deve ser removido.  
   **Status:** Passou

5. **Adicionar produtos ao carrinho e verificar se o número de itens no carrinho é atualizado**

   **Passos:** Na visualização do carrinho, verifique se a quantidade é atualizada.  
   **Resultado obtido:** Ao adicionar produtos, o carrinho está sendo atualizado.  
   **Resultado esperado:** O carrinho deve sempre ser atualizado ao adicionar um novo produto.  
   **Status:** Passou

6. **Verificar se ao clicar em "continuar comprando", a plataforma retorna para a página inicial com os produtos**

   **Passos:** Na visualização do carrinho, clique em "Continuar comprando".  
   **Resultado obtido:** Ao clicar em "Continuar comprando", a plataforma retornou para a página inicial.  
   **Resultado esperado:** A plataforma deve retornar para a página inicial ao clicar em "Continuar comprando".  
   **Status:** Passou

### Casos de teste: Etapa 5 - Fluxo completo de compra (do carrinho até finalização)

1. **Verificar se ao clicar em "checkout", o usuário é direcionado para a tela de informações da compra**

   **Passos:** Clique em checkout e visualize as informações da compra.  
   **Resultado obtido:** Ao clicar em checkout, o usuário visualiza as informações da compra.  
   **Resultado esperado:** Ao clicar em checkout, o usuário deve visualizar as informações da compra.  
   **Status:** Passou

2. **Verificar se é possível inserir as informações para a compra (primeiro nome, sobrenome e CEP)**

   **Passos:** Em informações da compra, clique para inserir suas informações.  
   **Resultado obtido:** Ao tentar inserir o primeiro nome, a tela carregou e ficou em branco.  
   **Resultado esperado:** Deve ser possível inserir os dados para a compra.  
   **Ajuste/Bug:** A plataforma está apresentando falha ao tentar inserir as informações da compra. Ao clicar no campo, a página fica em branco, dessa forma não está sendo possível prosseguir com os testes.  
   **Status:** Necessário ajuste

3. **Adicionar produtos ao carrinho e verificar se o número de itens no carrinho é atualizado**

   **Passos:** Adicione vários produtos ao carrinho e verifique se a quantidade é atualizada.  
   **Resultado obtido:** Ao inserir produtos no carrinho, a quantidade está sendo atualizada corretamente.  
   **Resultado esperado:** A quantidade adicionada no carrinho deve estar de acordo com o que foi inserido pelo usuário.  
   **Status:** Passou

4. **Navegar até a página de checkout e verificar os dados de pagamento e envio**

   **Passos:** Navegue até a tela de checkout e visualize os dados de pagamento e envio.  
   **Resultado obtido:** As informações de pagamento, envio e total estão sendo exibidas, mas não é possível visualizar o endereço de entrega do produto.  
   **Resultado esperado:** Antes de finalizar a compra, devem ser apresentadas as informações de pagamento, informações do endereço de envio e o total a ser pago.  
   **Ajuste:** Inserir informação de endereço.  
   **Status:** Necessário ajuste

5. **Finalizar a compra e verificar se a página de confirmação é exibida**

   **Passos:** Clique para finalizar a compra.  
   **Resultado obtido:** Ao clicar para finalizar a compra, a página de confirmação está sendo apresentada corretamente.  
   **Resultado esperado:** Ao finalizar a compra, o usuário deve ser redirecionado para a tela de compra concluída.  
   **Status:** Passou

6. **Verificar se na página de finalização da compra está sendo exibido o botão com a opção para clicar e retornar à página inicial**

   **Passos:** Na página de finalização da compra, verifique se está sendo apresentado o botão para retornar à página inicial.  
   **Resultado obtido:** O botão está sendo apresentado na página de finalização da compra e sendo possível clicar para retornar à página inicial.  
   **Resultado esperado:** Deve ser apresentado um botão clicável para retornar à página inicial dos produtos.  
   **Status:** Passou

### Casos de teste: Etapa 6 - Rede social (navegação dos ícones)

1. **Verificar se ao clicar nos ícones de navegação, o mesmo está sendo redirecionado corretamente ao link correspondente**

   ###### Twitter  
   **Status:** Passou

   ###### Facebook  
   **Status:** Passou

   ###### LinkedIn  
   **Status:** Passou

### Casos de teste: Etapa 7 - Menu lateral

1. **Verificar clique no menu lateral (abertura e fechamento de menu)**  
   **Status:** Passou

2. **Verificar se ao clicar em "todos os itens", o usuário é direcionado à página com todos os itens**  
   **Status:** Passou

3. **Verificar se ao clicar em "sobre", o usuário é direcionado para a página correspondente**  
   **Status:** Passou

4. **Verificar se é possível realizar "Logout"**  
   **Status:** Passou

### Bugs

- A plataforma está apresentando falha ao tentar inserir as informações da compra. Ao clicar no campo, a página fica em branco, dessa forma não está sendo possível prosseguir com os testes.

## Análise de Riscos

- Se o sistema falhar em processar o pagamento, isso pode resultar em perda de vendas.

### Melhorias Backend

**Etapa 1 - Login**
1. Login com senha inválida: Traduzir mensagem de retorno para português.
2. Login com usuário inválido: Traduzir mensagem de retorno para português.
3. Inserir limitação de caracteres nos campos usuário e senha.

**Etapa 2 - Ordenação e filtragem de produtos**
1. Aplicar corretamente a filtragem de A a Z e de Z a A.

**Etapa 5 - Fluxo completo de compra (do carrinho até finalização)**
1. A plataforma está apresentando falha ao tentar inserir as informações da compra. Ao clicar no campo, a página fica em branco, dessa forma não está sendo possível prosseguir com os testes.  
   **Observação:** Essa ação não acontece com frequência.  
2. Inserir informação de endereço na finalização da compra.

### Melhorias Frontend

**Etapa 1 - Login**
1. Função de ícone "x" para apagar o texto por completo não está funcional nos campos usuário e senha. A função de ícone "x" só funciona no retorno da mensagem de erro.
2. Ajustar layout do retorno da resposta. Quando o retorno de texto é maior que 20 caracteres, o layout está quebrando.

**Etapa 5 - Fluxo completo de compra (do carrinho até finalização)**
1. A plataforma está apresentando falha ao tentar inserir as informações da compra. Ao clicar no campo, a página fica em branco, dessa forma não está sendo possível prosseguir com os testes.  
   **Observação:** Essa ação não acontece com frequência.  
2. Inserir informação de endereço na finalização da compra.

### Melhorias de UX/UI

**Etapa 1 - Login**
1. Melhorar visualização do ícone "x", deixar um padrão que combine melhor com a tela inicial da plataforma.

**Etapa 4 - Adicionar e remover do carrinho**  
1. Inserir modal que seja possível editar a quantidade de produto ao invés de só visualizar a quantidade.
   
