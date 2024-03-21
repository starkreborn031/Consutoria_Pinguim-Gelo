# Passo 1: Escolha do Protocolo VPN

O OpenVPN é uma escolha popular devido à sua segurança e flexibilidade. Ele é compatível com várias plataformas e oferece recursos avançados de criptografia.

## Passo 2: Instalação e Configuração do Servidor OpenVPN

1. **Escolha do Sistema Operacional:** Dependendo do sistema operacional do servidor (Linux, Windows, etc.), você pode encontrar tutoriais específicos online.
2. **O SISTEMA OPERACIONAL DO CLIENTE É WINDOWS**

### Passo 3: Geração de Certificados de Cliente

1. **Criação de Certificados:** Utilize a ferramenta Easy-RSA (incluída na instalação do OpenVPN) para gerar os certificados de cliente.

>./clean-all
>./build-ca
>./build-key-server server
>./build-key client_name
> **Siga as instruções para preencher os detalhes do certificado.**

### **Assinatura do Certificado:** *Após gerar os certificados de cliente, assine-os no servidor OpenVPN para validação*

> /sign-req client client_name
> **Isso criará o certificado e a chave para o cliente.**

#### Passo 4: Configuração do Firewall/Roteador

No firewall/roteador da empresa, você precisa permitir o tráfego VPN encaminhando as portas necessárias para o servidor OpenVPN. Por exemplo, se estiver usando o protocolo UDP na porta 1194 (padrão do OpenVPN), você deve configurar o roteador para encaminhar o tráfego UDP da porta 1194 para o endereço IP do servidor OpenVPN.

### Passo 5: Fornecimento do Cliente OpenVPN ao Usuário

Forneça ao usuário o cliente OpenVPN correspondente ao sistema operacional da máquina dele (Windows, etc.). Além disso, forneça os certificados gerados no Passo 3, incluindo o arquivo de configuração do cliente (geralmente um arquivo `.ovpn`).

Espero que essa aula tenha sido útil para você entender como configurar uma VPN utilizando o OpenVPN. Certifique-se de ajustar os detalhes conforme necessário para a infraestrutura específica da sua empresa e siga as práticas recomendadas de segurança ao lidar com certificados e configurações de rede.
