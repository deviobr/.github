# 📦 Packages - Devio NPM Packages

## 🚀 O que são?

A **Devio** utiliza diversos pacotes privados para auxiliar no desenvolvimento, padronizar processos e evitar retrabalho com tarefas repetitivas.

---

## 🔐 Como acessar os pacotes?

Para instalar os pacotes privados, é necessário gerar um **GitHub Personal Access Token**.  
Siga os passos abaixo:

---

### 🔧 Gerando o Token no GitHub

1. Clique no seu **avatar** (canto superior direito) e vá em `Settings`  
   ![settings](images/settings.png)

2. No menu lateral, vá até o final da página e clique em `Developer settings`  
   ![developer settings](images/developer_settings.png)

3. Clique em `Personal access tokens`, depois selecione `Tokens (classic)`  
   ![token clássico](images/classic_token.png)

4. Clique em `Generate new token` e selecione `Classic`

5. Configure o token:
   - Dê um nome como: `NPM_DEVIO_TOKEN`
   - Em **expiration**, escolha `No expiration` (preferencialmente)
   - Marque as permissões conforme a imagem:  
     ![permissões de acesso](images/token_access.png)

6. Após gerar, copie o token e execute os comandos abaixo no terminal:

```bash
npm config set @deviobr:registry https://npm.pkg.github.com
npm config set //npm.pkg.github.com/:_authToken=${NPM_DEVIO_TOKEN}
```

---

### 🌐 Configurando a variável de ambiente `NPM_DEVIO_TOKEN`

A variável precisa ser adicionada ao sistema para uso contínuo.  
O processo varia conforme o sistema operacional:

#### 💻 Linux / macOS

1. Edite o arquivo `~/.bashrc`, `~/.zshrc` ou `~/.bash_profile` e adicione:

```bash
export NPM_DEVIO_TOKEN=<SEU_TOKEN>
```

2. Aplique a alteração:

```bash
source ~/.bashrc
# ou
source ~/.zshrc
```

3. Verifique:

```bash
echo $NPM_DEVIO_TOKEN
```

#### 🪟 Windows (PowerShell)

1. Execute o comando abaixo para adicionar a variável:

```powershell
[System.Environment]::SetEnvironmentVariable("NPM_DEVIO_TOKEN", "<SEU_TOKEN>", "Machine")
```

2. Verifique se a variável foi criada corretamente:

```powershell
echo $env:NPM_DEVIO_TOKEN
```

---

Pronto! Agora você pode instalar e utilizar os pacotes privados da Devio com segurança e praticidade.  
Para dúvidas, procure o time responsável.