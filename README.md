## Criação do banco de dados

```
CREATE TABLE [dbo].[Contatos](
	[id] [int] IDENTITY(1,1) NOT NULL,
	[nome] [nchar](100) NULL,
	[endereco] [nchar](200) NULL,
	[celular] [nchar](15) NULL,
	[telefone] [nchar](15) NULL,
	[email] [nchar](100) NULL,
 CONSTRAINT [PK_Contatos] PRIMARY KEY CLUSTERED 
(
	[id] ASC
)WITH (PAD_INDEX = OFF, STATISTICS_NORECOMPUTE = OFF, IGNORE_DUP_KEY = OFF, ALLOW_ROW_LOCKS = ON, 
ALLOW_PAGE_LOCKS = ON) ON [PRIMARY]
) ON [PRIMARY]
GO
```

## Alteração da conexão com banco de dados

```
SqlConnection con = new SqlConnection(@"Data Source=(localdb)\Local;Initial Catalog=Cadastro_Agenda;Integrated Security=True");
```

## Exemplo Agenda
Este exemplo utiliza conexão com banco de dados local e uma estrutura básica de crud para manipulação de dados

<img src="https://cdn.discordapp.com/attachments/1046824853015113789/1202495119970926612/image.png?ex=65cda9d9&is=65bb34d9&hm=ff97fda6d7f8b10c73c7723e0995390f1626e5153baeef7c2ea40da29be7f6c0&" alt="Logo da Minha Empresa">



