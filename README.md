<H1 align="center">CRUD Schedule</H1>
<p align="center">🚀 Development of CRUD in C# for future references.</p>


## Example Schedule
This example uses a local database connection and a basic crud structure for data manipulation

<div align="center">
<img src="https://github.com/lucasmargui/CSHARP_AGENDA_CRUD/assets/157809964/8479848f-c72b-4fe2-a535-346541fd8252" style="width:90%">
</div>

## Database create

<details>
   <summary>Click to show content</summary>
  
```
CREATE TABLE [dbo].[Contacts](
[id] [int] IDENTITY(1,1) NOT NULL,
[name] [nchar](100) NULL,
[address] [nchar](200) NULL,
[mobile] [nchar](15) NULL,
[phone] [nchar](15) NULL,
[email] [nchar](100) NULL,
  CONSTRAINT [PK_Contacts] PRIMARY KEY CLUSTERED
(
[id] ASC
)WITH (PAD_INDEX = OFF, STATISTICS_NORECOMPUTE = OFF, IGNORE_DUP_KEY = OFF, ALLOW_ROW_LOCKS = ON,
ALLOW_PAGE_LOCKS = ON) ON [PRIMARY]
) ON [PRIMARY]
GO
```

</details>

## Changing the database connection

```
SqlConnection con = new SqlConnection(@"Data Source=(localdb)\Local;Initial Catalog=Cadastro_Agenda;Integrated Security=True");
```

