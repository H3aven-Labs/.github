## PR Checklist

Você:
- [ ] Commitou o arquivo de deploy para o postgres? (se tiver tido alterações no prisma)
- [ ] Certificou que os testes estão passando localmente?
- [ ] Certificou que os testes estão passando na pipeline?
- [ ] Validou que as rotas não quebram quando subem para o cloudformation? (se tiver tido alterações nas rotas)

### Se tiver atualizado uma variável do .env
- [ ] Registrou ela no .env.sample?
- [ ] Registrou ela no .env.e2e-test?
- [ ] Atualizou o Dockerfile e docker-compose.dev.yml?
- [ ] Atualizou o valor default dela no h3-devops?
- [ ] Rodou o [Workflow de atualização das secrets](https://github.com/H3aven-Labs/h3-devops/actions/workflows/create-update-github-secrets.yml) no h3-devops depois do passo acima?
- [ ] Vai lembrar de gerar uma nova versão do docker com essa atualização depois que essa PR for aprovada?