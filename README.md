# Asturias: law history in git

The law of the autonomous community of Asturias (Comunidad Autónoma del Principado de Asturias, Spain) as a git history: one file per article, one commit per norm that changed it, dated the day the change took effect, with the amending norm as the commit's author. `git blame` names the norm behind every paragraph; `git log` lists every change to an article; checking out a date gives the text in force that day.

It follows the shared design of [lexifina/global-law](https://github.com/lexifina/global-law), which places it at `es-as/`. Spain's national law is in [lexifina/spain-law](https://github.com/lexifina/spain-law).

The text is in Spanish, exactly as the BOE's consolidated text prints it. Texts in co-official languages are not included.

Basado en datos de la Agencia Estatal Boletín Oficial del Estado (<https://www.boe.es>). Every text here is a consolidated text for information only (texto consolidado de carácter meramente informativo), not an official publication.

## What this repository holds

140 norms with 463 versions so far: the Estatuto de Autonomía first, then the laws, decree-laws and legislative decrees in force that the BOE consolidates, oldest first, added in parts of about 50. 17 of them are repealed norms the BOE consolidates: their whole history is kept, and their last commit removes the text on the day the repeal took effect, credited to the repealing norm. Regulations are not included (the BOE consolidates no autonomic decrees or orders).

| Folder | Norm | Versions | History | BOE last updated |
| --- | --- | ---: | --- | --- |
| `estatuto-de-autonomia/` | Ley Orgánica 7/1981, de 30 de diciembre, de Estatuto de Autonomía para Asturias. | 7 | as first published, then each change: 31 January 1982 to 18 July 2010 | 2026-10-23 |
| `ley-1983-004/` | Ley 4/1983, de 4 de agosto, reguladora del procedimiento de designación de Senadores por el Principado de Asturias. | 2 | as first published, then each change: 10 August 1983 to 29 January 1991 | 2025-12-16 |
| `ley-1984-001/` | Ley 1/1984, de 27 de abril, por la que se establece el Himno del Principado y se regula su uso. | 1 | as first published: 24 May 1984 | 2025-12-16 |
| `ley-1984-002/` | Ley 2/1984, de 27 de abril, por la que se establece el Escudo del Principado y se regula su uso. | 1 | as first published: 24 May 1984 | 2025-12-16 |
| `ley-1984-004/` | Ley 4/1984, de 5 de junio, reguladora de la iniciativa legislativa de los Ayuntamientos y de la iniciativa popular. | 1 | as first published: 28 June 1984 | 2026-10-23 |
| `ley-1984-005/` | Ley 5/1984, de 28 de junio, por la que se instituye el Día de Asturias. | 1 | as first published: 7 July 1984 | 2025-12-16 |
| `ley-1984-006/` | Ley 6/1984, de 5 de julio, del Presidente y del Consejo de Gobierno del Principado de Asturias. | 8 | as first published, then each change: 12 July 1984 to 24 December 2018 | 2025-12-16 |
| `ley-1984-007/` | Ley 7/1984, de 13 de julio, de Relaciones entre el Consejo de Gobierno y la Junta General del Principado de Asturias. | 1 | as first published: 12 August 1984 | 2025-12-16 |
| `ley-1984-011/` | Ley 11/1984, de 15 de octubre, de Salud Escolar para el Principado de Asturias. | 2 | as first published, then each change: 22 October 1984 to 1 May 2019 | 2025-12-16 |
| `ley-1985-001/` | Ley 1/1985, de 4 de junio, reguladora de la publicación de las normas, así como de las disposiciones y otros actos de los órganos del Principado de Asturias. | 1 | as first published: 7 July 1985 | 2025-12-16 |
| `ley-1986-003/` | Ley 3/1986, de 15 de mayo, por la que se regula el procedimiento de creación de Comarcas en el Principado de Asturias. | 1 | as first published: 19 June 1986 | 2025-12-17 |
| `ley-1986-004/` | Ley 4/1986, de 15 de mayo, Reguladora de los Honores y Distinciones del Principado de Asturias. | 2 | as first published, then each change: 19 June 1986 to 19 April 2022 | 2025-12-17 |
| `ley-1986-010/` | Ley 10/1986, de 7 de noviembre, reguladora de la Demarcación Territorial de los Concejos del Principado de Asturias. | 1 | as first published: 8 December 1986 | 2025-12-17 |
| `ley-1986-011/` | Ley 11/1986, de 20 de noviembre, por la que se reconoce la personalidad jurídica de la parroquia rural. | 1 | as first published: 24 December 1986 | 2025-12-17 |
| `ley-1986-014/` | Ley 14/1986, de 26 de diciembre, sobre régimen de elecciones a la Junta General del Principado de Asturias. | 2 | as first published, then each change: 2 February 1987 to 28 March 1991 | 2025-12-17 |
| `ley-1988-002/` | Ley 2/1988, de 10 de junio por la que se declara el Parque Natural de Somiedo. | 3 | as first published, then each change: 18 July 1988 to 2 December 2017 | 2025-12-17 |
| `ley-1988-008/` | Ley 8/1988, de 13 de diciembre, por la que se autoriza la modificación de los Estatutos de la Fundación Pública «Centro Regional de Bellas Artes», y se crea el Organismo autónomo Orquesta Sinfónica del Principado de Asturias. | 3 | as first published, then each change: 24 January 1989 to 1 January 2004 | 2025-12-17 |
| `ley-1989-001/` | Ley 1/1989, de 18 de abril, por la que se determina la capitalidad de los partidos judiciales comprendidos en el ámbito territorial del Principado de Asturias. | 1 | as first published: 17 May 1989 | 2025-12-17 |
| `ley-1989-002/` | Ley 2/1989, de 6 de junio, de caza. | 5 | as first published, then each change: 7 July 1989 to 16 May 1999 | 2026-02-03 |
| `ley-1989-004/` | Ley 4/1989, de 21 de julio, de Ordenación Agraria y Desarrollo Rural. | 4 | as first published, then each change: 10 September 1989 to 1 January 2015 | 2025-12-17 |
| `ley-1990-004/` | Ley 4/1990, de 19 de diciembre, de la Bandera del Principado de Asturias. | 1 | as first published: 10 January 1991 | 2026-02-26 |
| `ley-1990-007/` | Ley 7/1990, de 29 de diciembre, de Presupuestos Generales del Principado de Asturias para 1991. | 2 | as first published, then each change: 1 January 1991 to 1 January 1997 | 2025-12-17 |
| `ley-1991-001/` | Ley 1/1991, de 21 de febrero, de Patrimonio del Principado de Asturias. | 8 | as first published, then each change: 27 March 1991 to 22 December 2025 | 2025-12-17 |
| `ley-1991-005/` | Ley 5/1991, de 5 de abril, de Protección de los Espacios Naturales. | 5 | as first published, then each change: 7 May 1991 to 4 December 2021 | 2025-12-17 |
| `ley-1991-007/` | Ley 7/1991, de 5 de abril, de asistencia y protección al anciano. | 6 | as first published, then each change: 9 May 1991 to 25 July 2014 | 2026-09-08 |
| `ley-1991-008/` | Ley 8/1991, de 30 de julio, de Organización de la Administración del Principado de Asturias. | 6 | as first published, then each change: 25 August 1991 to 22 December 2025 | 2025-12-17 |
| `ley-1991-009/` | Ley 9/1991, de 30 de diciembre, por la que se establece un recargo sobre las cuotas mínimas del Impuesto sobre Actividades Económicas. | 1 | as first published: 1 January 1992 | 2025-12-17 |
| `ley-1993-002/` | Ley 2/1993, de 29 de octubre, de pesca marítima en aguas interiores y aprovechamiento de recursos marinos. | 2 | as first published, then each change: 5 December 1993 to 1 January 2003 | 2025-12-17 |
| `ley-1994-001/` | Ley 1/1994, de 21 de febrero, sobre Abastecimiento y Saneamiento de Aguas en el Principado de Asturias. | 17 | as first published, then each change: 17 March 1994 to 13 April 2023 | 2025-12-17 |
| `ley-1995-001/` | Ley 1/1995, de 27 de enero, de protección del menor. | 2 | as first published, then each change: 1 March 1995 to 1 January 2020 | 2026-10-23 |
| `ley-1995-002/` | Ley 2/1995, de 13 de marzo, sobre régimen jurídico de la Administración del Principado de Asturias. | 10 | as first published, then each change: 4 April 1995 to 22 December 2025 | 2025-12-18 |
| `ley-1995-003/` | Ley 3/1995, de 15 de marzo, de Sanciones en Materia de Vivienda. | 3 | as first published, then each change: 18 April 1995 to 1 January 2003 | 2025-12-18 |
| `ley-1995-005/` | Ley 5/1995, de 6 de abril, de promoción de la accesibilidad y supresión de barreras. | 2 | as first published, then each change: 9 May 1995 to 30 June 2021 | 2025-12-18 |
| `ley-1996-005/` | Ley 5/1996, de 27 de diciembre, de creación del Colegio Profesional de Protésicos Dentales del Principado de Asturias. | 1 | as first published: 20 January 1997 | 2025-12-18 |
| `ley-1996-007/` | Ley 7/1996, de 27 de diciembre, de creación del Colegio Profesional de Podólogos del Principado de Asturias. | 1 | as first published: 20 January 1997 | 2025-12-18 |
| `ley-1996-008/` | Ley 8/1996, de 27 de diciembre, de Declaración del Parque Natural de Redes. | 4 | as first published, then each change: 20 January 1997 to 10 December 2017 | 2025-12-18 |
| `ley-1996-009/` | Ley 9/1996, de 27 de diciembre, reguladora del Consejo Escolar del Principado de Asturias. | 2 | as first published, then each change: 1 January 1997 to 20 May 2018 | 2025-12-18 |
| `ley-1997-001/` | Ley 1/1997, de 4 de abril, de infracciones y sanciones en materia de seguridad minera. | 2 | as first published, then each change: 24 July 1997 to 11 July 2026 | 2026-07-17 |
| `ley-1997-002/` | Ley 2/1997, de 16 de julio, del Consejo Social de la Universidad de Oviedo. | 1 | as first published: 2 August 1997 | 2025-12-18 |
| `ley-1997-005/` | Ley 5/1997, de 18 de diciembre, de academias en el ámbito del Principado de Asturias. | 1 | as first published: 19 January 1998 | 2025-12-18 |
| `ley-1998-001/` | Ley 1/1998, de 23 de marzo, de uso y promoción del bable/asturiano. | 1 | as first published: 17 April 1998 | 2025-12-18 |
| `decreto-legislativo-del-principado-de-asturias-1998-001/` | Decreto Legislativo del Principado de Asturias 1/1998, de 11 de junio, por el que se aprueba el texto refundido de las Leyes de Tasas y de Precios Públicos. | 23 | as first published, then each change: 27 June 1998 to 1 January 2026 | 2026-02-09 |
| `decreto-legislativo-1998-002/` | Decreto Legislativo 2/1998, de 25 de junio, por el que se aprueba el texto refundido del Régimen Económico y Presupuestario. | 27 | as first published, then each change: 3 July 1998 to 1 January 2026 | 2026-02-09 |
| `ley-1999-005/` | Ley 5/1999, de 29 de marzo, por la que se crea el Servicio Regional de Investigación y Desarrollo Agroalimentario del Principado de Asturias. | 3 | as first published, then each change: 29 April 1999 to 12 January 2023 | 2025-12-18 |
| `ley-2000-001/` | Ley 1/2000, de 20 de junio, por la que se crea la Comisión Asturiana de Administración Local. | 1 | as first published: 30 June 2000 | 2025-12-18 |
| `ley-2000-002/` | Ley 2/2000, de 23 de junio, de Cajas de Ahorro. | 5 | as first published, then each change: 7 July 2000 to 25 December 2010 | 2025-12-18 |
| `ley-2001-001/` | Ley 1/2001, de 6 de marzo, del Patrimonio Cultural. | 16 | as first published, then each change: 19 April 2001 to 1 January 2026 | 2026-02-09 |
| `ley-2001-007/` | Ley 7/2001, de 22 de junio, de Turismo. | 5 | as first published, then each change: 7 July 2001 to 20 November 2024 | 2025-12-18 |
| `ley-2001-008/` | Ley 8/2001, de 15 de octubre, de regulación del Servicio Público de Atención de Llamadas de Urgencia y de Creación de la Entidad Pública "112 Asturias". | 3 | as first published, then each change: 21 October 2001 to 1 August 2013 | 2025-12-18 |
| `ley-2001-009/` | Ley 9/2001, de 15 de octubre, de creación de la entidad pública «Bomberos del Principado de Asturias». | 4 | as first published, then each change: 21 October 2001 to 1 August 2013 | 2025-12-18 |
| `ley-del-principado-de-asturias-2001-010/` | Ley del Principado de Asturias 10/2001, de 12 de noviembre, del Voluntariado. | 1 | as first published: 17 November 2001 | 2026-04-30 |
| `ley-2002-001/` | Ley 1/2002, de 11 de marzo, del Consorcio de Transportes de Asturias. | 3 | as first published, then each change: 24 March 2002 to 1 January 2026 | 2026-02-09 |
| `ley-2002-002/` | Ley 2/2002, de 12 de abril, del Instituto de Desarrollo Económico del Principado de Asturias. | 2 | as first published, then each change: 30 May 2002 to 12 January 2023 | 2025-12-18 |
| `ley-2002-004/` | Ley 4/2002, de 23 de mayo, de Parejas Estables. | 1 | as first published: 1 June 2002 | 2025-12-18 |
| `ley-2002-005/` | Ley 5/2002, de 3 de junio, sobre vertidos de aguas residuales industriales a los sistemas públicos de saneamiento. | 2 | as first published, then each change: 4 July 2002 to 13 April 2023 | 2025-12-18 |
| `ley-2002-006/` | Ley 6/2002, de 18 de junio, sobre protección de los ecosistemas acuáticos y de regulación de la pesca en aguas continentales. | 1 | as first published: 1 October 2002 | 2025-12-18 |
| `ley-2002-008/` | Ley 8/2002, de 21 de octubre, de Espectáculos Públicos y Actividades Recreativas. | 3 | as first published, then each change: 24 December 2002 to 4 June 2026 | 2026-05-25 |
| `ley-2002-009/` | Ley 9/2002, de 22 de octubre, de la Reserva Natural Integral de Muniellos. | 1 | as first published: 24 November 2002 | 2025-12-18 |
| `ley-2002-011/` | Ley 11/2002, de 2 de diciembre, de los Consumidores y Usuarios. | 2 | as first published, then each change: 13 January 2003 to 1 January 2007 | 2025-12-18 |
| `ley-2002-012/` | Ley 12/2002, de 13 de diciembre, de declaración del Parque Natural de las Fuentes del Narcea, Degaña e Ibias. | 5 | as first published, then each change: 16 January 2003 to 2 December 2017 | 2025-12-18 |
| `ley-2002-013/` | Ley 13/2002, de 23 de diciembre, de tenencia, protección y derechos de los animales. | 1 | as first published: 20 January 2003 | 2025-12-18 |
| `ley-2002-015/` | Ley 15/2002, de 27 de diciembre, de Medidas Presupuestarias, Administrativas y Fiscales. | 12 | as first published, then each change: 1 January 2003 to 1 January 2015 | 2025-12-18 |
| `ley-2003-001/` | Ley 1/2003, de 24 de febrero, de servicios sociales. | 5 | as first published, then each change: 9 March 2003 to 14 April 2019 | 2026-03-20 |
| `ley-2003-003/` | Ley 3/2003, de 24 de marzo, de la Sindicatura de Cuentas. | 4 | as first published, then each change: 23 April 2003 to 9 April 2015 | 2026-04-22 |
| `ley-2003-004/` | Ley 4/2003, de 24 de marzo, de declaración del Parque Natural de Ponga. | 3 | as first published, then each change: 4 April 2003 to 2 December 2017 | 2025-12-18 |
| `decreto-legislativo-2004-001/` | Decreto Legislativo 1/2004, de 22 de abril, por el que se aprueba el texto refundido de las disposiciones legales vigentes en materia de ordenación del territorio y urbanismo. | 9 | as first published, then each change: 28 April 2004 to 28 December 2024 | 2025-12-18 |
| `ley-2004-001/` | Ley 1/2004, de 21 de octubre, del Consejo Consultivo. | 3 | as first published, then each change: 24 November 2004 to 28 February 2006 | 2025-12-18 |
| `ley-2004-002/` | Ley 2/2004, de 29 de octubre, de medidas urgentes en materia de suelo y vivienda. | 5 | as first published, then each change: 11 November 2004 to 1 January 2007 | 2025-12-18 |
| `ley-2004-003/` | Ley 3/2004, de 23 de noviembre, de montes y ordenación forestal. | 5 | as first published, then each change: 3 March 2005 to 22 December 2025 | 2025-12-18 |
| `ley-2004-004/` | Ley 4/2004, de 30 de noviembre, del Instituto Asturiano de Prevención de Riesgos Laborales. | 1 | as first published: 2 January 2005 | 2025-12-18 |
| `ley-2005-003/` | Ley 3/2005, de 8 de julio, del Servicio Público de Empleo. | 1 | as first published: 18 October 2005 | 2026-04-01 |
| `ley-2006-004/` | Ley 4/2006, de 5 de mayo, de Cooperación al Desarrollo. | 1 | as first published: 8 June 2006 | 2025-12-18 |
| `ley-2006-005/` | Ley 5/2006, de 30 de mayo, del Parque Natural de Las Ubiñas-La Mesa. | 3 | as first published, then each change: 25 June 2006 to 2 December 2017 | 2025-12-18 |
| `ley-2006-006/` | Ley 6/2006, de 20 de junio, de Comunicación y Publicidad Institucionales. | 1 | as first published: 21 July 2006 | 2025-12-18 |
| `ley-2006-007/` | Ley 7/2006, de 3 de noviembre, de Estadística. | 2 | as first published, then each change: 7 December 2006 to 1 June 2013 | 2025-12-19 |
| `ley-2006-008/` | Ley 8/2006, de 13 de noviembre, de Carreteras. | 4 | as first published, then each change: 13 December 2007 to 22 December 2025 | 2025-12-19 |
| `ley-2007-001/` | Ley 1/2007, de 16 de marzo, de atención y ordenación farmacéutica. | 2 | as first published, then each change: 27 April 2007 to 26 March 2018 | 2025-12-19 |
| `ley-2007-002/` | Ley 2/2007, de 23 de marzo, de Coordinación de las Policías Locales. | 3 | as first published, then each change: 30 April 2007 to 11 May 2024 | 2025-12-19 |
| `ley-2007-003/` | Ley 3/2007, de 23 de marzo, de Mediación Familiar. | 1 | as first published: 9 October 2007 | 2025-12-19 |
| `ley-2009-006/` | Ley 6/2009, de 29 de diciembre, de Evaluación de la Función Docente y sus Incentivos. | 2 | as first published, then each change: 1 January 2010 to 1 January 2017 | 2025-12-19 |
| `ley-2010-002/` | Ley 2/2010, de 12 de marzo, de integración del "Hospital del Oriente de Asturias Francisco Grande Covián" y de su personal en el Servicio de Salud del Principado de Asturias en régimen de gestión directa. | 1 | as first published: 20 March 2010 | 2025-12-19 |
| `ley-2010-009/` | Ley 9/2010, de 17 de diciembre, de comercio interior. | 3 | as first published, then each change: 25 December 2010 to 25 July 2014 | 2025-12-19 |
| `ley-2011-002/` | Ley 2/2011, de 11 de marzo, para la igualdad de mujeres y hombres y la erradicación de la violencia de género. | 1 | as first published: 7 April 2011 | 2026-04-13 |
| `ley-2013-001/` | Ley 1/2013, de 24 de mayo, de medidas de reestructuración del sector público autonómico. | 1 | as first published: 1 June 2013 | 2025-12-19 |
| `ley-2013-003/` | Ley 3/2013, de 28 de junio, de medidas de autoridad del profesorado. | 1 | as first published: 5 July 2013 | 2025-12-19 |
| `ley-2014-005/` | Ley 5/2014, de 6 de junio, de extinción de la Cámara Agraria del Principado de Asturias. | 1 | as first published: 19 June 2014 | 2025-12-19 |
| `ley-2014-006/` | Ley 6/2014, de 13 de junio, de Juego y Apuestas. | 4 | oldest version available, then each change: 17 July 2014 to 8 September 2022 | 2025-12-19 |
| `ley-2014-008/` | Ley 8/2014, de 17 de julio, de segunda reestructuración del sector público autonómico. | 1 | as first published: 25 July 2014 | 2025-12-19 |
| `decreto-legislativo-2014-001/` | Decreto Legislativo 1/2014, de 23 de julio, por el que se aprueba el texto refundido de las disposiciones legales del Principado de Asturias en materia de tributos propios. | 6 | as first published, then each change: 1 January 2015 to 1 January 2021 | 2026-04-24 |
| `decreto-legislativo-2014-002/` | Decreto Legislativo 2/2014, de 22 de octubre, por el que se aprueba el texto refundido de las disposiciones legales del Principado de Asturias en materia de tributos cedidos por el Estado. | 21 | as first published, then each change: 30 October 2014 to 1 January 2026 | 2026-02-09 |
| `ley-2015-001/` | Ley 1/2015, de 20 de febrero, de Creación del Colegio Profesional de Terapeutas Ocupacionales. | 1 | as first published: 3 April 2015 | 2025-12-19 |
| `ley-2015-004/` | Ley 4/2015, de 6 de marzo, de atención integral en materia de drogas y bebidas alcohólicas. | 2 | as first published, then each change: 20 May 2015 to 13 July 2017 | 2025-12-19 |
| `ley-2015-008/` | Ley 8/2015, de 20 de marzo, de Cámaras Oficiales de Comercio, Industria, Servicios y Navegación. | 1 | as first published: 9 April 2015 | 2025-12-19 |
| `ley-2016-002/` | Ley 2/2016, de 1 de julio, de medidas financieras y de gestión presupuestaria y de creación de tarifas por expedición de licencias interautonómicas de caza y pesca. | 1 | as first published: 8 July 2016 | 2025-12-19 |
| `ley-2018-002/` | Ley 2/2018, de 23 de marzo, de los asturianos en el exterior y del reconocimiento de la asturianía. | 1 | as first published: 6 May 2018 | 2025-12-20 |
| `ley-2018-005/` | Ley 5/2018, de 22 de junio, sobre derechos y garantías de la dignidad de las personas en el proceso del final de la vida. | 1 | as first published: 4 October 2018 | 2025-12-20 |
| `ley-2018-006/` | Ley 6/2018, de 18 de julio, de creación del Colegio Profesional de Dietistas-Nutricionistas. | 1 | as first published: 25 August 2018 | 2025-12-20 |
| `ley-2018-007/` | Ley 7/2018, de 24 de julio, de medidas en materia de función pública como consecuencia de la prórroga presupuestaria. | 1 | as first published: 28 July 2018 | 2025-12-20 |
| `ley-2018-008/` | Ley 8/2018, de 14 de septiembre, de Transparencia, Buen Gobierno y Grupos de Interés. | 2 | as first published, then each change: 24 December 2018 to 22 December 2025 | 2025-12-20 |
| `ley-2018-011/` | Ley 11/2018, de 16 de noviembre, de la Inspección General de Servicios. | 1 | as first published: 1 January 2019 | 2025-12-20 |
| `ley-2018-012/` | Ley 12/2018, de 23 de noviembre, de Transportes y Movilidad Sostenible. | 2 | as first published, then each change: 24 December 2018 to 4 December 2021 | 2025-12-20 |
| `ley-2019-001/` | Ley 1/2019, de 1 de marzo, para la recuperación de la memoria democrática en el Principado de Asturias. | 1 | as first published: 9 March 2019 | 2025-12-20 |
| `ley-2019-002/` | Ley 2/2019, de 1 de marzo, de calidad alimentaria, calidad diferenciada y venta directa de productos alimentarios. | 1 | as first published: 28 March 2019 | 2025-12-20 |
| `ley-2019-003/` | Ley 3/2019, de 15 de marzo, sobre acción concertada con entidades de iniciativa social sin ánimo de lucro para la prestación de servicios de carácter social. | 1 | as first published: 14 April 2019 | 2025-12-20 |
| `ley-2019-006/` | Ley 6/2019, de 29 de marzo, de Participación y Promoción Juvenil. | 1 | as first published: 1 June 2019 | 2025-12-20 |
| `ley-2019-007/` | Ley 7/2019, de 29 de marzo, de Salud. | 7 | as first published, then each change: 1 May 2019 to 10 May 2025 | 2025-12-20 |
| `ley-2020-002/` | Ley 2/2020, de 23 de diciembre, reguladora del derecho de acceso al entorno de las personas usuarias de perros de asistencia. | 1 | as first published: 30 June 2021 | 2026-10-09 |
| `ley-2021-001/` | Ley 1/2021, de 5 de mayo, de creación del Colegio Profesional de Economistas de Asturias por fusión del Colegio de Economistas de Asturias y del Colegio Oficial de Titulados Mercantiles y Empresariales de Asturias. | 1 | as first published: 20 June 2021 | 2025-12-20 |
| `ley-2021-003/` | Ley 3/2021, de 30 de junio, de Garantía de Derechos y Prestaciones Vitales. | 3 | as first published, then each change: 12 July 2022 to 29 September 2026 | 2026-10-06 |
| `ley-2021-004/` | Ley 4/2021, de 1 de diciembre, de Medidas Administrativas Urgentes. | 3 | as first published, then each change: 4 December 2021 to 13 April 2023 | 2025-12-20 |
| `ley-2022-003/` | Ley 3/2022, de 18 de mayo, por la que se aprueba el Plan Asturiano de Estadística 2022-2025. | 1 | as first published: 1 June 2022 | 2025-12-20 |
| `ley-2022-005/` | Ley 5/2022, de 29 de junio, de Actividad Física y Deporte. | 1 | as first published: 8 September 2022 | 2025-12-20 |
| `ley-2022-006/` | Ley 6/2022, de 29 de junio, del Real Instituto de Estudios Asturianos. | 1 | as first published: 28 July 2022 | 2025-12-20 |
| `ley-2022-009/` | Ley 9/2022, de 30 de noviembre, de la Agencia de Ciencia, Competitividad Empresarial e Innovación. | 1 | as first published: 12 January 2023 | 2025-12-20 |
| `ley-2023-001/` | Ley 1/2023, de 15 de marzo, de Calidad Ambiental. | 4 | as first published, then each change: 13 April 2023 to 1 January 2026 | 2026-02-09 |
| `ley-2023-002/` | Ley 2/2023, de 15 de marzo, de Empleo Público. | 2 | as first published, then each change: 25 April 2023 to 26 March 2025 | 2025-12-20 |
| `ley-2024-002/` | Ley 2/2024, de 30 de abril, de Impulso Demográfico. | 2 | as first published, then each change: 11 May 2024 to 22 December 2025 | 2026-04-13 |
| `ley-2024-005/` | Ley 5/2024, de 13 de noviembre, por la que se establece la Red Autonómica de Escuelas Infantiles, se regula su extensión y la integración en la misma de las Escuelas Infantiles Municipales. | 1 | as first published: 20 November 2024 | 2025-12-20 |
| `ley-2024-007/` | Ley 7/2024, de 20 de diciembre, de Proyectos de Interés Estratégico. | 1 | as first published: 28 December 2024 | 2025-12-20 |
| `ley-2025-001/` | Ley 1/2025, de 19 de febrero, de Ciencia, Tecnología e Innovación. | 1 | as first published: 26 March 2025 | 2025-12-20 |
| `ley-del-principado-de-asturias-2026-001/` | Ley del Principado de Asturias 1/2026, de 18 de marzo, del Estatuto de las Mujeres Rurales del Principado de Asturias. | 1 | as first published: 19 April 2026 | 2026-04-23 |
| `ley-del-principado-de-asturias-2026-003/` | Ley del Principado de Asturias 3/2026, de 13 de mayo, de Colegios Profesionales. | 1 | as first published: 18 June 2026 | 2026-06-11 |
| `ley-del-principado-de-asturias-2026-004/` | Ley del Principado de Asturias 4/2026, de 28 de mayo, de Cooperativas. | 1 | as first published: 10 August 2026 | 2026-06-22 |
| `ley-1984-003/` | Ley 3/1984, de 9 de mayo, de reconocimiento de la asturianía. | 3 | as first published, then each change: 18 May 1984 to 6 May 2018; **repealed** 6 May 2018 by Ley 2/2018, de 23 de marzo (BOE-A-2018-5998) | 2025-12-16 |
| `ley-1985-003/` | Ley 3/1985, de 26 de diciembre, de Ordenación de la Función Publica de la Administración del Principado de Asturias. | 19 | as first published, then each change: 19 January 1986 to 25 April 2023; **repealed** 25 April 2023 by Ley 2/2023, de 15 de marzo (BOE-A-2023-10348) | 2025-12-17 |
| `ley-1986-001/` | Ley 1/1986, de 31 de marzo, del Consejo de la Juventud del Principado de Asturias. | 2 | as first published, then each change: 9 April 1986 to 1 June 2019; **repealed** 1 June 2019 by Ley 6/2019, de 29 de marzo (BOE-A-2019-7840) | 2025-12-17 |
| `ley-1988-007/` | Ley 7/1988, de 5 de diciembre, por la que se reorganiza el Instituto de Estudios Asturianos. | 2 | as first published, then each change: 22 December 1988 to 28 July 2022; **repealed** 28 July 2022 by Ley 6/2022, de 29 de junio (BOE-A-2022-11962) | 2025-12-17 |
| `ley-1990-005/` | Ley 5/1990, de 19 de diciembre, sobre prohibición de venta de bebidas alcohólicas a menores de dieciséis años. | 2 | as first published, then each change: 29 January 1991 to 20 May 2015; **repealed** 20 May 2015 by Ley 4/2015, de 6 de marzo (BOE-A-2015-4847) | 2026-07-09 |
| `ley-1992-001/` | Ley 1/1992, de 2 de julio, del Servicio de Salud del Principado de Asturias. | 7 | as first published, then each change: 2 August 1992 to 1 May 2019; **repealed** 1 May 2019 by Ley 7/2019, de 29 de marzo (BOE-A-2019-7841) | 2026-03-06 |
| `ley-1992-002/` | Ley 2/1992, de 30 de diciembre, del Impuesto sobre el Juego del Bingo. | 2 | as first published, then each change: 14 January 1993 to 1 January 2015; **repealed** 1 January 2015 by Decreto Legislativo 1/2014, de 23 de julio (BOE-A-2015-944) | 2025-12-17 |
| `ley-1994-002/` | Ley 2/1994, de 29 de diciembre, del deporte. | 2 | as first published, then each change: 3 February 1995 to 8 September 2022; **repealed** 8 September 2022 by Ley 5/2022, de 29 de junio (BOE-A-2022-11961) | 2025-12-18 |
| `ley-1995-004/` | Ley 4/1995, de 6 de abril, de incompatibilidades, actividades y bienes de los altos cargos del Principado de Asturias. | 2 | as first published, then each change: 9 May 1995 to 24 December 2018; **repealed** 24 December 2018 by Ley 8/2018, de 14 de septiembre (BOE-A-2018-14293) | 2025-12-18 |
| `ley-1997-003/` | Ley 3/1997, de 24 de noviembre, de la Cámara Agraria del Principado de Asturias. | 2 | as first published, then each change: 21 December 1997 to 19 June 2014; **repealed** 19 June 2014 by Ley 5/2014, de 6 de junio (BOE-A-2014-9264) | 2025-12-18 |
| `ley-2001-002/` | Ley 2/2001, de 27 de marzo, del Consejo Económico y Social. | 4 | as first published, then each change: 5 April 2001 to 7 November 2017; **repealed** 7 November 2017 by Ley 8/2017, de 27 de octubre (BOE-A-2017-13749) | 2025-12-18 |
| `ley-2001-003/` | Ley 3/2001, de 4 de mayo, de Juego y Apuestas. | 6 | as first published, then each change: 15 May 2001 to 17 July 2014; **repealed** 17 July 2014 by Ley 6/2014, de 13 de junio (BOE-A-2014-9265) | 2025-12-18 |
| `ley-2003-002/` | Ley 2/2003, de 17 de marzo, de Medios de Comunicación Social. | 5 | as first published, then each change: 13 April 2003 to 25 July 2014; **repealed** 25 July 2014 by Ley 8/2014, de 17 de julio (BOE-A-2014-10577) | 2025-12-18 |
| `ley-2005-004/` | Ley 4/2005, de 28 de octubre, de Salario Social Básico. | 5 | as first published, then each change: 24 November 2005 to 12 July 2022; **repealed** 12 July 2022 by Ley 3/2021, de 30 de junio (BOE-A-2021-13685) | 2025-12-18 |
| `ley-2010-004/` | Ley 4/2010, de 29 de junio, de Cooperativas. | 3 | as first published, then each change: 1 August 2010 to 10 August 2026; **repealed** 10 August 2026 by Ley del Principado de Asturias 4/2026, de 28 de mayo (BOE-A-2026-13298) | 2026-08-09 |
| `ley-2014-001/` | Ley 1/2014, de 14 de abril, del Impuesto sobre las Afecciones Ambientales del Uso del Agua. | 2 | as first published, then each change: 1 May 2014 to 1 January 2015; **repealed** 1 January 2015 by Decreto Legislativo 1/2014, de 23 de julio (BOE-A-2015-944) | 2025-12-19 |
| `ley-2018-010/` | Ley 10/2018, de 2 de noviembre, de categorías profesionales del personal estatutario del Servicio de Salud del Principado de Asturias. | 2 | as first published, then each change: 10 November 2018 to 1 May 2019; **repealed** 1 May 2019 by Ley 7/2019, de 29 de marzo (BOE-A-2019-7841) | 2025-12-20 |

## Source

The consolidated legislation of the Agencia Estatal Boletín Oficial del Estado (BOE), through its open-data API, <https://www.boe.es/datosabiertos/api/legislacion-consolidada>. For each consolidated norm it gives every block of the text (article, disposition, annex, heading) with every version of that block, the day each version took effect (fecha_vigencia) and the norm that made it (id_norma). Each version here is the whole text as it stood on one of those days. The last column above is the BOE's own last-update date for the consolidated text.

## Dates

- Each commit is dated at **noon, Europe/Madrid, on the day the change took effect**: the fecha_vigencia the BOE gives the new block versions.
- A day on which the BOE records a new block version that changes no words is not a version here.
- Block versions with no in-force date (the BOE's 99999999, a date not yet fixed) are left out.
- An act's first commit is its first publication when the BOE's earliest text is the act as enacted; otherwise it is the oldest version the BOE holds.
- Versions that take effect after the retrieval day are on the `futuro` branch, never merged into `main`.

## Files

`<act>/art-005.md` is Artículo 5, `art-005-bis.md` Artículo 5 bis; `da-01.md` the Disposición adicional primera, `dt-` transitional, `dd-` repealing and `df-` final dispositions (`-unica` for "única"); `preambulo.md` the preamble, `firma.md` the signature, `anexo-*.md` the annexes. The book, title, chapter and section headings sit at the top of the file of the article that follows them. One paragraph per line; a table one line per row, cells separated by ` | `.

## How it is checked

- Every version of every act is read back from git on the day it took effect and on the day before (`tools/check_repo.py`); both must match `corpus.json`.
- The letters and digits of every version equal those of the BOE's own text of that day, rebuilt from the source XML by a separate reader, and every file's text appears in it.
- Health checks: no merge commits, commit dates never go backwards, nothing dated in the future, and every commit's trailers parse.

## What "author" means

The author of a commit is the norm that changed the text (a law, a decree-law, a ruling of the Constitutional Court), named by its title and BOE identifier, with an e-mail address that cannot exist (`<boe id>@boe.es.invalid`). The committer is always Lexifina.

## Limits

This is not an official publication. Only the texts published in the official journals are authentic. The history starts with the oldest text the BOE consolidates for each norm. Only the norms listed above are included; norms the BOE does not consolidate are not.
