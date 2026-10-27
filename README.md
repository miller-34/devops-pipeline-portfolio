# DevOps Pipeline Portfolio

Portfólio de projetos práticos de DevOps, automação, CI/CD,
containerização, Kubernetes, GitOps e observabilidade.

O objetivo é demonstrar a implementação de pipelines automatizados,
práticas de segurança, implantação de aplicações e monitoramento
de serviços.

## Projeto em destaque: DevOps Node API

API desenvolvida em Node.js, com testes automatizados e pipeline
de integração e entrega contínuas.

**Repositório:** [devops-node-api](https://github.com/miller-34/devops-node-api)

### Tecnologias utilizadas

- Node.js e Express
- Jest e testes automatizados com cobertura
- Docker e GitHub Container Registry (GHCR)
- GitHub Actions para CI/CD
- Trivy para análise de vulnerabilidades
- Kubernetes para orquestração
- Argo CD para GitOps
- Prometheus para coleta de métricas
- Grafana para visualização e observabilidade

### Pipeline CI/CD

O workflow executa as seguintes etapas:

1. **Tests & Coverage** — executa os testes automatizados e verifica a cobertura.
2. **Docker Build** — constrói e valida a imagem da aplicação.
3. **Security Scan** — analisa vulnerabilidades da imagem com Trivy.
4. **Publish to GHCR** — publica a imagem no GitHub Container Registry.

![Pipeline CI/CD](https://raw.githubusercontent.com/miller-34/devops-node-api/main/docs/images/github-actions-pipeline.png)

### Kubernetes e GitOps

Os manifestos Kubernetes ficam versionados no repositório da aplicação.
O Argo CD acompanha a configuração GitOps e sincroniza os recursos
declarados no Git com o cluster.

![Aplicação sincronizada no Argo CD](https://raw.githubusercontent.com/miller-34/devops-node-api/main/docs/images/argocd-gitops.png)

### Observabilidade

O dashboard Grafana apresenta indicadores da aplicação, incluindo:

- Status dos pods
- Taxa de requisições HTTP
- Requisições por código de resposta
- Latência HTTP P95
- Consumo de memória por pod
- Consumo de CPU por pod

![Dashboard de observabilidade](https://raw.githubusercontent.com/miller-34/devops-node-api/main/docs/images/grafana-observability.png)

## Competências demonstradas

- Automação de testes e pipelines CI/CD
- Construção e publicação de imagens Docker
- Análise de vulnerabilidades
- Versionamento e revisão de configurações
- Orquestração com Kubernetes
- GitOps com Argo CD
- Monitoramento com Prometheus e Grafana
- Documentação técnica e evidências de implementação

## Repositórios

- [DevOps Node API](https://github.com/miller-34/devops-node-api)
- [DevOps Pipeline Portfolio](https://github.com/miller-34/devops-pipeline-portfolio)

---

Portfólio em evolução, com foco em automação, confiabilidade,
segurança e boas práticas de engenharia.
