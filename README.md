# 🛡️ Relatório de Incidente de Segurança: Análise de Rede

## 📝 Descrição do Projeto
Este projeto foi desenvolvido como parte da minha formação em Segurança Cibernética. O foco foi a investigação de um incidente envolvendo o site `yummyrecipesforme.com`, utilizando análise de tráfego de rede para identificar vulnerabilidades e propor correções.

## 🔍 Resumo do Incidente
Identificamos que um invasor utilizou um ataque de **força bruta** para comprometer uma conta administrativa que utilizava uma senha padrão. O atacante injetou um script malicioso que redirecionava usuários para um domínio falso (`greatrecipesforme.com`) para distribuição de malware.

## 🛠️ Ferramentas e Conceitos Aplicados
* **Análise de Pacotes:** Uso de `tcpdump` para inspecionar o tráfego.
* **Protocolos de Rede:** Identificação de HTTP (Camada de Aplicação), DNS e TCP.
* **Ambiente Controlado:** Uso de *Sandbox* para análise de malware sem risco à rede local.



[Image of TCP/IP model layers]


## 🛡️ Remediação e Prevenção
Com base na análise, as recomendações de segurança incluem:
* **MFA (Autenticação de Dois Fatores):** Para neutralizar ataques de força bruta.
* **Políticas de Senha:** Bloqueio de senhas padrão e exigência de complexidade.
* **Limitação de Tentativas:** Implementação de bloqueio de conta após sucessivas falhas de login.

## 📂 Arquivos
* [Visualizar Relatório Completo (PDF)](./relatorios/Exemplo-de-relatorio.pdf)

* ---

## 💡 Análise do Exemplar (Lógica Técnica)
Além do relatório final, este projeto incluiu um estudo sobre a fundamentação das respostas:

* **Análise do Protocolo:** O uso do HTTP foi confirmado pela observação do tráfego na porta 80 e pela natureza do serviço web afetado.
* **Análise da Documentação:** A estruturação seguiu um padrão factual, detalhando desde a causa raiz (Brute Force) até o vetor de ataque (JavaScript Injection).
* **Análise da Remediação:** As soluções propostas focam em controles de acesso robustos para impedir que vulnerabilidades de credenciais padrão sejam exploradas novamente.

---
