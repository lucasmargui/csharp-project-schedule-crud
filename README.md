<H1 align="center">Agenda CRUD</H1>
<p align="center">🚀 Desenvolvimento de estrutura de CRUD em C# para referências futuras.</p>


## Criação do banco de dados

<details>
  <summary>Clique para mostrar conteúdo</summary>
  
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

</details>



## Alteração da conexão com banco de dados


```
SqlConnection con = new SqlConnection(@"Data Source=(localdb)\Local;Initial Catalog=Cadastro_Agenda;Integrated Security=True");
```

## Exemplo Agenda
Este exemplo utiliza conexão com banco de dados local e uma estrutura básica de crud para manipulação de dados



<div align="center">
<img src="https://github.com/lucasmargui/CSHARP_AGENDA_CRUD/assets/157809964/8479848f-c72b-4fe2-a535-346541fd8252" style="width:90%">
</div>





