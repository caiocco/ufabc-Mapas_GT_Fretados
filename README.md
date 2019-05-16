![Logotipo da UFABC](icones/ufabc.png?raw=true)

# Introdução

## Propósito

Este repositório abriga arquivos da produção cartográfia desempenhada por mim para auxílio ao grupo de trabalho (GT) que se formou em torno da questão do fretado da Universidade Federal do ABC (UFABC), que passou a seguir mais rigorosamente o anacrônico marco regulatório existente, tendo sua capacidade degradada.

O GT então passa a buscar articulação junto a outros indivíduos e entidades, de forma a sugerir aprimoramento no transporte intermunicipal sob responsabilidade da EMTU (Empresa Metropolitana de Transportes Urbanos).

## Observações importantes

Este conteúdo **não tem** afiliação direta com a UFABC, nem é apoiado e/ou representa a opinião da Reitoria. Trata-se de um esforço de um aluno sob demanda do GT.

Opiniões e análises que possam vir a ser publicadas no âmbito do [COMMU (Coletivo Metropolitano de Mobilidade Urbana)](https://medium.com/@commu) **não necessariamente representam as visões da comunidade acadêmica, entidades e do supracitado grupo de trabalho**.

Não reinvindico qualquer tipo de *copyright* sobre o conteúdo aqui disponibilizado, pois entendo que se trata de informação de caráter público, gerada a partir de dados abertos.

**Não forneço garantia de qualquer tipo, o uso dos arquivos aqui disponibilizados é por sua conta e risco.**

----------------

# Conteúdo do repositório

## Diretórios

[produtos](https://github.com/caiocco/ufabc-Mapas_GT_Fretados/tree/master/produtos): é aqui que são exportados os mapas em formatos abertos ou cujo padrão é disseminado, permitindo sua visualização e impressão por um público mais amplo, incluindo outras pessoas que pertencem ao GT.

[icones](https://github.com/caiocco/ufabc-Mapas_GT_Fretados/tree/master/icones): possui imagens vetoriais em formato SVG, utilizadas pelo QGIS como símbolos, caso deseje editar os ícones, você pode utilizar um software livre e de código aberto como o Inkscape.

[www.emtu.sp.gov.br](https://github.com/caiocco/ufabc-Mapas_GT_Fretados/tree/master/www.emtu.sp.gov.br): possui parte dos dados descarregados a partir do sítio da EMTU, incluindo dados GTFS ou gerados a partir dos dados do GTFS. Nem todo o conteúdo está disponível no GitHub devido ao tamanho máximo de arquivo permitido (25 MB), porém, todo o conteúdo necessário está disponível, de forma que qualquer pessao interessada pode reconstruir e editar os mapas, desde que tenha os conhecimentos ou interesse em desenvolver as habilidades necessárias.

[www.ibge.gov.br](https://github.com/caiocco/ufabc-Mapas_GT_Fretados/tree/master/www.ibge.gov.br/sp_municipios): possui dados descarregados a partir do FTP do IBGE, necessários para o desenho das feições dos municípios da Região Metropolitana de São Paulo.

[www.openstreetmap.org](https://github.com/caiocco/ufabc-Mapas_GT_Fretados/tree/master/www.openstreetmap.org): dados extraídos do OpenStreetMap, um projeto de mapeamento aberto, essencial para obter o traçado de algumas linhas do município de São Bernardo do Campo. A utilização assume que você possui os complementos OSMDownloader e QuickOSM habilitados e funcionando no QGIS.

## Arquivos

O arquivo `README.md` contém o arquivo LEIA-ME que está sendo exibido e lido por você. Trata-se de texto formatado em linguagem Markdown.

Os arquivos com o padrão `principais_pontos.*` correspondem ao *shapefile* de pontos que mapeia alguns locais-chave no contexto do trabalho, como estações da CPTM (Companhia Paulista de Trens Metropolitanos) e campi da UFABC.

O arquivo `mapa_emtu.qgz` é o arquivo de projeto do QGIS no formato atual, que adota compressão. O arquivo possui todas as camadas necessárias, incluindo camadas auxiliares, além disso, todos os mapas exportáveis estão presentes no compositor. A utilização do arquivo e das funcionalidades do QGIS exige conhecimento intermediário, a depender das edições desejadas.

----------------

# Como utilizar os dados aqui disponibilizados

Caso não tenha familiaridade com o GitHub e o sistema de versionamento Git, informo que [você pode baixar todos os dados de uma vez num arquivo compactado](https://github.com/caiocco/ufabc-Mapas_GT_Fretados/archive/master.zip).

Recomenda-se a utilização de computador pessoal de arquitetura x86 de 64 bits, executando alguma distribuição Linux capaz de rodar a última versão do QGIS. Foi utilizado o Fedora 29 Workstation em máquina virtual, com QGIS 3.6.2, hospedado no openSUSE Leap 43.2. O hardware recomendado pode ter cerca de 10 anos de idade, desde que possua memória RAM suficiente e subsistema de armazenamento massivo devidamente dimensionado, considerando um cenário de virtualização similar ao adotado por mim, fica recomendado:

* Pelo menos 2,5 GB de RAM para a máquina virtual (para rodar o QGIS num ambiente como o Xfce)
* Pelo menos 8 GB de RAM no hospedeiro, lembrando que mais de 2 GB vão ser usados só para a máquina virtual
* Disco veloz (ou SSD) ou dois discos lentos em RAID-0 ou RAID-1
* Uma distribuição estável como hospedeira, como openSUSE Leap ou CentOS

Sumário com detalhes do computador utilizado para geoprocessamento (modificado a partir de *output* do software HardInfo):

```
-Computer-
Processor: 4x Intel(R) Xeon(R) CPU E5-1607 0 @ 3.00GHz
Memory: 12254MB (9619MB used)
Operating System: openSUSE 42.3 (x86_64)
-Display-
Resolution: 1680x1050 pixels
OpenGL Renderer: GeForce 210/PCIe/SSE2
-SCSI Disks-
ATA ST3000DM001-1ER1
ATA ST3000DM001-1ER1
TSSTcorp DVD+-RW SN-208BB
TSSTcorp CD/DVDW SH-W162L
-Operating System Version-
Kernel: Linux 4.4.176-96-default (x86_64)
Compiled: #1 SMP Fri Mar 22 06:23:26 UTC 2019 (a0dd1b8)
C Library: GNU C Library version 2.22 (git bbab82c25da9) (stable)
Default C Compiler: GNU C Compiler version 4.8.5 (SUSE Linux) 
Distribution: openSUSE 42.3 (x86_64)
-Current Session-
Desktop Environment: Unknown (Window Manager: FVWM)
```

O detalhamento das recomendações está muito além do escopo do LEIA-ME.