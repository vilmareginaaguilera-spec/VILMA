# Desafio DevSecOps — Gerenciador de Tarefas

## Sobre o Projeto
Este repositório faz parte do desafio prático do módulo de DevSecOps da ADA Tech.
Você receberá este projeto com vulnerabilidades propositais e uma pipeline incompleta.
Seu objetivo é **implementar a pipeline de segurança** e **corrigir as vulnerabilidades**.

## Estado atual
A pipeline está **incompleta**. Os steps de segurança precisam ser implementados por você.

## Sua missão
1. Implementar os steps de segurança no `pipeline.yml`
2. Fazer a pipeline **quebrar** ao detectar os problemas
3. Corrigir as vulnerabilidades encontradas
4. Fazer a pipeline **passar** com tudo verde ✅
5. Documentar o funcionamento da pipeline neste README

## O que implementar
- [ ] Secrets Scanning com **Gitleaks**
- [ ] SAST com **Semgrep**
- [ ] SCA com **Grype**
- [ ] Deploy com **GitHub Pages**

## Como a pipeline funciona
> **Substitua este bloco pela sua explicação após implementar a pipeline.**
> 
> ### Step 3 — Secrets Scanning (Gitleaks)
- **O que faz:** Escaneia o código e histórico de commits em busca de segredos expostos (senhas, tokens, chaves de API).
- **Por que é importante:** Evita que credenciais sensíveis sejam publicadas no repositório e exploradas por atacantes.
- **Resultado:** Se encontrar segredos, a pipeline **quebra** imediatamente.

### Step 4 — SAST (Semgrep)
- **O que faz:** Analisa o código estaticamente em busca de padrões inseguros (XSS, SQL Injection, uso de funções perigosas).
- **Por que é importante:** Detecta falhas de segurança antes mesmo de o código rodar em produção.
- **Resultado:** Se encontrar vulnerabilidades, a pipeline **quebra**.
- 
- ### Step 5 — SCA (Grype)
- **O que faz:** Verifica as dependências do projeto contra uma base de CVEs (vulnerabilidades conhecidas).
- **Por que é importante:** Dependências desatualizadas ou vulneráveis são uma das maiores fontes de ataques.
- **Resultado:** A pipeline **quebra** se encontrar vulnerabilidades de severidade **média ou maior**.

### Step 6 — Deploy (GitHub Pages)
- **O que faz:** Publica automaticamente o projeto no GitHub Pages.
- **Por que é importante:** Garante que apenas código seguro chegue à produção.
- **Resultado:** Só acontece se todos os steps anteriores passarem.

## URL de Produção
> (https://github.com/vilmareginaaguilera-spec/VILMA)
