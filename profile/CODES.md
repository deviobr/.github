# 📦 Codes - Ferramenta de Deploy Automatizado

## ✅ O que é?

**Codes** é uma ferramenta automatizada de deploy utilizada para os ambientes de **desenvolvimento**, **homologação** e **produção**.  
Esse sistema acessa diversas máquinas via **SSH** e torna os projetos públicos na internet de forma prática e segura.

---

## 🔐 Como acessar?

1. Acesse: [https://devio.codes](https://devio.codes)
2. Faça login com sua conta Devio (`seu.nome@devio.com.br`).
3. Para iniciar um novo projeto:
   - Solicite ao seu gestor a criação de um ambiente.
   - Ou peça para ser convidado em um projeto já existente pela sua equipe.

---

## 👥 Quem utiliza o Codes?

### 🔎 QA (Quality Assurance)
- Utilizam os ambientes de **homologação** criados pelos desenvolvedores para testes controlados.
- Isso garante maior fidelidade entre o ambiente de testes e o ambiente final.

### 👨‍💻 Desenvolvedores
- Em projetos com mais de um membro, todos podem utilizar o ambiente compartilhado para integrações e validações.
- Mantenha sempre o ambiente **limpo** e **ativo**.

### 🤝 Clientes
- Têm acesso ao ambiente durante o desenvolvimento, com entregas parciais feitas a cada sprint.
- O ambiente do cliente deve ser **separado** do QA para evitar conflitos de dados e instabilidades.
- Apenas funcionalidades **validadas pelo QA** devem estar disponíveis para o cliente.

---

## 🛠️ O cliente contratou suporte. E agora?

- Para clientes com **suporte contratado**, utilizamos **máquinas separadas** do ambiente padrão do Codes.
- É necessário adicionar um novo **destination** dentro do Codes.
- **Nunca** coloque projetos de clientes em produção junto ao Codes sem **autorização prévia**.
- O ambiente de produção do cliente deve ser criado pelo gestor e vinculado ao Codes apenas para deploys.

---

## ⚠️ Avisos Importantes

- ⏰ O Codes desliga **automaticamente às 22h** e reinicia às **7h**, visando economia de custos.
  - Se precisar de mais tempo, avise seu gestor para manter o ambiente ativo.
- 🧩 Os bancos de dados configurados como `public` podem apresentar instabilidades ao ativar o acesso externo.
  - Se isso ocorrer, **ative e desative** o switch algumas vezes até funcionar.
- 📁 Atualmente, todos os projetos (**front-end**, **back-end** e **banco de dados**) são alocados no Codes.

---

Para dúvidas ou problemas, entre em contato com o time responsável.