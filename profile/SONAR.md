# 🔍 SonarQube - Análise de Qualidade de Código

## ✅ O que é?

**SonarQube** é uma ferramenta de análise estática de código utilizada para auxiliar desenvolvedores na aplicação de boas práticas, como os princípios **SOLID**.  
Ela fornece **feedbacks automáticos** e **métricas** importantes sobre a qualidade, segurança e manutenibilidade do código.

---

## 📊 Indicadores

![Métricas do Sonar](images/sonar_metrics.png)

- **Security**: Trechos do código que podem conter falhas de segurança.
- **Reliability**: Código com baixo padrão de legibilidade ou potencialmente instável.
- **Maintainability**: Trechos que requerem manutenção devido à complexidade, tamanho ou má estrutura.
- **Hotspots Reviewed**: Trechos com possíveis dados sensíveis, falhas lógicas ou problemas de sintaxe.
- **Coverage**: Percentual de cobertura de testes (unitários, componentes e integração).
- **Duplications**: Percentual de código duplicado no projeto.

---

## 🎯 Métricas na Devio

Na **Devio**, seguimos algumas metas padrão para garantir qualidade nos projetos:

| Indicador           | Meta                                                  |
| ------------------- | ----------------------------------------------------- |
| **Security**        | Manter em **0**                                       |
| **Reliability**     | Manter em **0**                                       |
| **Maintainability** | Abaixo de **100 itens**                               |
| **Hotspots**        | Todos devem ser **revisados** antes de nova varredura |
| **Coverage**        | Mínimo de **10%**                                     |
| **Duplications**    | Abaixo de **15%**                                     |

> ⚠️ **Atenção**: Caso existam hotspots pendentes, a próxima verificação irá **quebrar** automaticamente.

---

## 🛠️ Como adicionar o Sonar ao seu projeto

Execute o comando abaixo para configurar automaticamente o Sonar no seu projeto. Ele adicionará os arquivos de configuração e o script de execução.

```bash
npx @deviobr/sonar
```

Para informações complementares acesse a documentação completa de [@deviobr/sonar](https://github.com/deviobr/-PACKAGE-CMS/pkgs/npm/cms)

Após a configuração, você poderá rodar o Sonar manualmente com:

```bash
npm run sonar
```

---

Para dúvidas ou suporte, entre em contato com o time responsável.
