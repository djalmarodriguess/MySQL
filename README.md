# MySQL
My studies on MySQL

#Banco de Dados "cursos"

CREATE TABLE `cursos` (
`idcurso` int(11) NOT NULL DEFAULT '0',
`nome` varchar(30) NOT NULL,
`descricao` text,
`carga` int(10) unsigned DEFAULT NULL,
`totaulas` int(10) unsigned DEFAULT NULL,
`ano` year(4) DEFAULT '2016',
PRIMARY KEY (`idcurso`),
UNIQUE KEY `nome` (`nome`)
) ENGINE=InnoDB DEFAULT CHARSET=utf8


#Banco de Dados "gafanhotos"

CREATE TABLE `gafanhotos` (
`id` int(11) NOT NULL AUTO_INCREMENT,
`nome` varchar(30) NOT NULL,
`profissao` varchar(20) DEFAULT NULL,
`nascimento` date DEFAULT NULL,
`sexo` enum('M','F') DEFAULT NULL,
`peso` decimal(5,2) DEFAULT NULL,
`altura` decimal(3,2) DEFAULT NULL,
`nacionalidade` varchar(20) DEFAULT 'Brasil',
PRIMARY KEY (`id`)
) ENGINE=InnoDB AUTO_INCREMENT=62 DEFAULT CHARSET=utf8


