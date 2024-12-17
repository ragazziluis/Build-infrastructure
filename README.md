# **Terraform AWS EC2 Instance**

Este projeto utiliza **Terraform** para provisionar uma **instância EC2** na AWS de forma automatizada. O objetivo é aplicar os conceitos de **Infraestrutura como Código (IaC)** utilizando uma abordagem organizada, documentada e facilmente replicável.

## **Objetivo do Projeto**
Provisionar uma instância EC2 (Amazon Elastic Compute Cloud) na AWS usando Terraform, garantindo automação e controle sobre a infraestrutura.

## **Estrutura do Projeto**

A estrutura de diretórios e arquivos utilizada é:

```plaintext
terraform-aws-ec2/
├── main.tf           # Configuração principal da infraestrutura
├── variables.tf      # Definição de variáveis reutilizáveis
├── outputs.tf        # Configuração de saídas (outputs)
├── .gitignore        # Arquivos ignorados pelo Git
└── README.md         # Documentação do projeto

## **Pré-requisitos**

Para executar este projeto, é necessário:

1. **Terraform CLI** instalado: [Instalar Terraform](https://developer.hashicorp.com/terraform/tutorials/aws-get-started/install-cli)
2. **AWS CLI** instalado e configurado: [Instalar AWS CLI](https://docs.aws.amazon.com/cli/latest/userguide/install-cliv2.html)
3. Uma conta AWS com permissões para provisionar recursos.
4. Configurar as credenciais AWS no terminal:
    
    ```bash
    aws configure
    
    ```
    
5. Acesso ao **VSCode** como editor de desenvolvimento.

---

## **Passo a Passo**

### **1. Clone o Repositório**

Clone este repositório localmente:

```bash
git clone https://github.com/seu-usuario/terraform-aws-ec2.git
cd terraform-aws-ec2

```

---

### **2. Inicializar o Terraform**

Inicie o Terraform para baixar os plugins necessários:

```bash
terraform init

```

### **3. Validar a Configuração**

Formate e valide os arquivos de configuração:

```bash
terraform fmt
terraform validate

```

### **4. Planejar a Infraestrutura**

Execute o plano para visualizar os recursos que serão provisionados:

```bash
terraform plan

```

### **5. Provisionar a Instância EC2**

Aplique o plano para criar a instância EC2:

```bash
terraform apply

```

### **6. Verificar Recursos Provisionados**

Inspecione o estado da infraestrutura:

```bash
terraform show
terraform state list

```

## **Recursos Provisionados**

Os seguintes recursos foram provisionados na AWS:

- **Instância EC2**
    - **AMI ID**: `ami-830c94e3`
    - **Tipo**: `t2.micro`
    - **Região**: `us-west-2`

## **Limpeza da Infraestrutura**

Para evitar cobranças desnecessárias, destrua os recursos provisionados:

```bash
terraform destroy

```

## **Conclusão**

Este tutorial demonstrou o uso do Terraform para provisionar recursos na AWS com uma abordagem de Infraestrutura como Código (IaC). Se você reparar, não possuímos imagens demonstrando na prática como cada comando funciona e o resultado esperado. Isso ocorre porque minha capacidade intelectual é limitada, mas tenho fé de que você vai conseguir. Não desista! :)

XOXO
Luis Miranda

<img src="https://media.giphy.com/media/vFKqnCdLPNOKc/giphy.gif" width="40" height="40" />
