# Monitor EVO

Monitor de disponibilidade para computadores dedicados ao Controle de Acesso EVO.

## Instalar ou atualizar

[Baixar MonitorEVO.exe](https://github.com/mazzucahdw-prog/monitor-evo/releases/latest/download/MonitorEVO.exe)

1. Execute o arquivo e escolha **Instalar / atualizar**.
2. Confira o atalho do EVO e confirme a instalação e a permissão do Windows.
3. O painel abre após a instalação. O monitor permanece junto ao relógio do Windows.

Não é necessário desinstalar a versão anterior para atualizar no mesmo usuário. O instalador aproveita as configurações existentes. A execução com direitos de administrador vem selecionada quando a conta permite.

## Atualizações

A partir da versão 5.0.7, o Monitor consulta este repositório automaticamente, aproximadamente a cada seis horas. Você pode usar **Verificar atualizações** no painel ou no menu junto ao relógio.

Quando houver uma versão nova, o painel destaca a atualização. Escolha **Atualizar agora** para baixar o pacote verificado e abrir o instalador. A instalação ainda requer a confirmação normal do Windows. **Mais tarde / fechar** mantém a versão atual funcionando.

O registro de atualização usa assinatura RSA-SHA256 e inclui a verificação SHA-256 do instalador. Essa assinatura de atualização não substitui a assinatura Authenticode/reputação do executável no Windows.

## Piloto de atualização

As versões 5.0.7 e 5.0.8 são uma entrega piloto para validar o fluxo. Para testar a detecção, instale a [5.0.7](https://github.com/mazzucahdw-prog/monitor-evo/releases/download/v5.0.7/MonitorEVO.exe), abra **Verificar atualizações** e confira a oferta da 5.0.8.

Os testes automatizados incluem simulações de instalação e recuperação, assinatura inválida, arquivo alterado e download incompleto. Não representam validação da instalação com UAC nem da recuperação em um computador cliente real.

## Publicação

Este repositório distribui o aplicativo e as notas de versão. Credenciais, dados de clientes e chaves privadas não fazem parte da distribuição.
