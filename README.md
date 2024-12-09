CREATE TABLE [dbo].[allSalesTable] (
[SaleID] INT           IDENTITY (1, 1) NOT NULL,
[Name]   VARCHAR (50)  NOT NULL,
[Price]  INT           NOT NULL,
[Qty]    INT           NOT NULL,
[Total]  VARCHAR (50)  NOT NULL,
[Date]   VARCHAR (100) NOT NULL,
PRIMARY KEY CLUSTERED ([SaleID] ASC)
);

CREATE TABLE [dbo].[AttTable] (
[AttID]    INT          IDENTITY (1, 1) NOT NULL,
[AttName]  VARCHAR (50) NOT NULL,
[Age]      INT          NOT NULL,
[Number]   INT          NOT NULL,
[Password] VARCHAR (50) NOT NULL,
PRIMARY KEY CLUSTERED ([AttID] ASC)
);

CREATE TABLE [dbo].[CatTable] (
[CatID]       INT           IDENTITY (1, 1) NOT NULL,
[CatName]     VARCHAR (100) NOT NULL,
[Description] VARCHAR (100) NOT NULL,
PRIMARY KEY CLUSTERED ([CatID] ASC)
);

CREATE TABLE [dbo].[historyTable] (
[ProdID]   INT          NOT NULL,
[ProdName] VARCHAR (50) NOT NULL,
[Quantity] INT          NOT NULL,
[Price]    INT          NOT NULL,
[Category] VARCHAR (50) NOT NULL,
PRIMARY KEY CLUSTERED ([ProdID] ASC)
);

CREATE TABLE [dbo].[ProdTable] (
[ProdID]   INT          IDENTITY (1, 1) NOT NULL,
[ProdName] VARCHAR (50) NOT NULL,
[Quantity] INT          NOT NULL,
[Price]    INT          NOT NULL,
[Category] VARCHAR (50) NOT NULL,
PRIMARY KEY CLUSTERED ([ProdID] ASC)

);
