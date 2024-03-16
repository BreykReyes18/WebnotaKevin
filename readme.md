CREATE TABLE `alumnos` (
  `Id_Alumno` int(8) NOT NULL AUTO_INCREMENT,
  `Nombre_Completo` varchar(50) DEFAULT NULL,
  `Cedula` varchar(20) DEFAULT NULL,
  `Direccion` text,
  `Telefono` varchar(20) DEFAULT NULL,
  `Carrera` varchar(20) DEFAULT NULL,
  `Turno` varchar(20) DEFAULT NULL,
  `Cursa` varchar(30) DEFAULT NULL,
  `Activo` varchar(2) DEFAULT NULL,
  PRIMARY KEY (`Id_Alumno`),
  UNIQUE KEY `Id_Alumno` (`Id_Alumno`)
) ENGINE=MyISAM DEFAULT CHARSET=utf8 PACK_KEYS=0;

CREATE TABLE `asignaturas` (
  `Id` int(11) NOT NULL AUTO_INCREMENT,
  `Codigo` varchar(10) DEFAULT NULL,
  `Asignaturas` varchar(50) DEFAULT NULL,
  `Facultad` varchar(50) DEFAULT NULL,
  `Horas_Teoricas` int(3) DEFAULT NULL,
  `Horas_Practicas` int(3) DEFAULT NULL,
  `Activo` varchar(2) DEFAULT NULL,
  PRIMARY KEY (`Id`),
  UNIQUE KEY `Id` (`Id`)
) ENGINE=MyISAM DEFAULT CHARSET=utf8 PACK_KEYS=0;

CREATE TABLE `usuarios` (
  `ID_Usuario` int(6) DEFAULT NULL,
  `Usuario` varchar(20) DEFAULT NULL,
  `Password` varchar(20) DEFAULT NULL,
  `Nombre_Usuario` varchar(20) DEFAULT NULL,
  `Tipo` varchar(20) DEFAULT NULL
) ENGINE=MyISAM DEFAULT CHARSET=utf8 PACK_KEYS=0;