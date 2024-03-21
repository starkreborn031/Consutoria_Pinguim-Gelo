# Configuração de Encaminhamento de Portas (**Port Forwarding**)

## *Passo 1*: Acesso às configurações do roteador/firewall

>1. Abra um navegador da web (como Google Chrome, Mozilla Firefox, etc.).
>2. Na barra de endereços do navegador, digite o endereço IP padrão do seu roteador/firewall. Você pode encontrar essa informação no manual do dispositivo. Por exemplo, pode ser algo como "192.168.1.1" ou "192.168.0.1". Pressione Enter.

## *Passo 2*: Localização da seção de encaminhamento de portas

1. **Após inserir o endereço IP, você será direcionado para a página de login do roteador/firewall. Faça login com as credenciais corretas. Geralmente, o nome de usuário padrão é "admin" e a senha pode ser "admin" ou estar em branco. Consulte o manual do dispositivo se não souber as credenciais.**

2. **Uma vez logado, navegue pelas opções ou guias disponíveis até encontrar a seção de encaminhamento de portas. Pode ser rotulado como "Port Forwarding", "Virtual Servers", "NAT Forwarding" ou algo semelhante, dependendo do fabricante e do modelo do dispositivo.**

## *Passo 3*: Criação da regra de encaminhamento de porta

1. Dentro da seção de encaminhamento de portas, procure por um botão ou opção para adicionar uma nova regra ou porta.

>2.Ao adicionar uma nova regra, você geralmente verá campos para preencher:
> -Nome da regra: dê um nome significativo para identificar a regra (por exemplo, "Impressora_Port_9100").
> -Protocolo: selecione o protocolo para o qual deseja encaminhar as portas (TCP, UDP ou ambos, dependendo das necessidades da sua impressora).
> -Porta de origem: geralmente deixada em branco para permitir qualquer porta de origem (ou insira uma porta específica, se necessário).
> -IP de destino: insira o endereço IP da sua impressora na rede local (por exemplo, "192.168.1.100").
> -Porta de destino: especifique a porta da impressora que deseja encaminhar (por exemplo, "9100" para impressão).
> -Salvar ou Aplicar: após preencher os campos necessários, salve ou aplique a nova regra.

## Final

>Depois de salvar a nova regra de encaminhamento de porta, o roteador/firewall começará a encaminhar as solicitações feitas para o IP público do roteador na porta específica da impressora (por exemplo, a porta 9100) para o IP local da impressora na rede. Certifique-se de que as configurações estejam corretas e teste a conexão para garantir que a impressora esteja acessível externamente.
>Lembre-se de que as interfaces de administração dos roteadores/firewalls podem variar um pouco entre os modelos e fabricantes, então os termos exatos e a localização das configurações podem diferir. Consultar o manual do dispositivo é sempre útil para obter instruções específicas para o seu equipamento.
