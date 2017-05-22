# EngSoft_TP1
Trabalho Prático 1 - Engenharia de Software 2 - Universidade Federal de Minas Gerais

<h2> Integrantes </h2>
  Breno Campos Ferreira Guimarães, César Augusto Moura Ferreira e João Paulo Martins Castanheira
  
<h2> Tópicos a serem tratados </h2>

1 - Descrição do sistema, incluindo principais features, objetivo, linguagem de programação.  
2 - Informações da equipe de desenvolvimento: principais desenvolvedores, funções na equipe (?)  
3 - Breve descrição da evolução do sistema: principais releases e novidades de cada uma.  
4 - Principais frameworks, ferramentas e linguagens usadas no desenvolvimento.  
5 - Documentação da arquitetura, na visão de "desenvolvimento" (modular), isto
é, principais módulos e suas responsabilidades, principais padrões de projeto
usados, justificativas para adoção dessa arquitetura etc. Se relevante,
documentar também visões de processo e física.  

[Wikipedia](https://en.wikipedia.org/wiki/VLC_media_player) - Vale a pena dar uma olhada

<h3> 1 - Descrição, features, objetivos e linguagens de programação </h3>

O VLC é um software livre de código aberto, dedicado a reproduzir, tocar e transmitir multimídia. A sigla VLC deriva de "VideoLAN Client", nome abandonado devido a incorporação do programa servidor (VideoLAN Server) no software cliente. O sistema dá suporta para uma ampla variedade de formatos de vídeo, tais como: OGM, MPEG1, MPEG-2, MPEG-4, DivX, DVD, VCDs etc. Os formatos de áudio também têm suporte para  OGG, Speex, FLAC, MPC (Musepack), MP3, WAV e outros. Usando tecnologias e bibliotecas open source, o VLC foi compatibilizado com a maioria das plataformas existentes, incluindo GNU/Linux, Windows, Mac OS X, BSD, iOS e Android.

Além disso o VLC suporta vários protocolos de transmissão em redes, podendo ser usado como servidor de video/audio em uma rede de alta velicidade, suportando tanto o unicast quanto o multicast operados em IPv4 ou IPv6.

Pelo motivo de o VLC usar transmissão baseada em pacotes, ele não reproduz os vídeos completamente. Ele lida com arquivos incompletos, pacotes danificados e outras particularidades da transferência de pacotes via peer-to-peer network (P2P). Ele também reproduz arquivos m2t MPEG(.TS) enquanto eles ainda estão sendo digitalizados de uma câmera HDV através de um cabo FireWire, tornando possível o monitoramento do do vídeo enquanto ele está sendo reproduzido. O tocador também utiliza a biblioteca libcdio (Compact Disc Input and Control library) que contém recursos para acesso para o CD-ROM e imagens de CD, o que possibilita o acesso aos arquivos .iso e assim reproduzindo conteúde de uma imagem de disco, mesmo se o sistema operacional do usuário não suportar o manuseio direto de arquivos deste formato.

O VLC suporta todos os tipode de áudio e vídeo suportados pelas bibliotecas libavcodec e libavformat, isso significa que o VLC pode tocar vídeos H.264 ou MPEG-4 Parte 2 como também suportar arquivosdo formato FLV ou MXF usando a biblioteca FFmpeg. O software pode reproduzir gravações de alta definição de fitas D-VHS (Digital Video Recording), como também transmitir ao vivo através da conexão por cabo FireWire videos não criptografados de um hardware de armazenamento para um monitor HDTV.

O reprodutor pode executar um vídeo diretamente no papel de parede da área de trabalho do windows, usando o DirectX. Recurso disponível apenas para o windows. Além dissso o VLC também oferece um screencast, recurso que grava em vídeo as atividades mostradas no output padrão do sistema operacional. É possível também fazer a conversão de mídia para uma ampla gama de formatos suportados. Finalmente o programa pode ser instalado ou reproduzir diretamente de um USB flash drive ou outra unidade externa. O VLC tem o código fonte escrito na linguagem de programação C e sua GUI (Graphic User Interface), escrita em C++ (com Qt) e Objective-C.

<h3> 2 - Equipe de Desenvolvimento </h3>

  A equipe do VLC conta com atuais 444 contribuidores ativos no mundo todo. Porém muito mais pessoas são lembradas e agradecidas no arquivo [AUTHORS](https://github.com/videolan/vlc/blob/master/AUTHORS) no diretório raíz do projeto. Entre estes estão 596 programadores, 13 artistas, uma pessoa responsável pela documentação.
  
  Entre os desenvolvedores supracitados, esta é a lista dos mais relevantes e/ou ativos na lista de contribuidores do projeto no GitHub:
  
1. [jbkempf](https://github.com/jbkempf) - 6,701 commits / 463,234 ++ / 604,582 --
2. [fcartegnie](https://github.com/fcartegnie) - 3,576 commits / 165,082 ++ / 116,866 --
3. [fkuehne](https://github.com/fkuehne) - 3,253 commits / 1,905,039 ++ / 2,568,959 --
4. [funman](https://github.com/funman) - 3,030 commits / 1,223,256 ++ / 457,569 --
5. [ivoire](https://github.com/ivoire) - 1,909 commits / 29,626 ++ / 45,410 --
6. [hartman](https://github.com/hartman) - 1,637 commits / 163,943 ++ / 158,529 --
7. [jpsaman](https://github.com/jpsaman) - 1,618 commits / 109,116 ++ / 49,024 --
8. [antoinecellerier](https://github.com/antoinecellerier) - 1,597 commits / 648,531 ++ / 439,734 --
9. [tguillem](https://github.com/tguillem) - 1,490 commits / 70,725 ++ / 44,329 --
10. [chouquette](https://github.com/chouquette) - 849 commits / 17,260 ++ / 12,984 --

A equipe de desenvolvimento do VLC, como citado anteriormente é formada por desenvolvedores do mundo todo e especialmente ex-estudantes da universidade École Centrale Paris. Abaixo alguns dos contribuidores mais relevantes e suas respectivas responsabilidades:

Billy Biggs - Aprimoramentos em libdvdcss  
Sven Heithecker - Manutenção do cache para discos com conteúdo identico mas chaves diferentes.  
Samuel Hocevar - Código original de descriptografia CSS do VCL  
Eugenio Jarosiewicz - MacOS X DVD ioctls.  
Jon Lech Johansen - Porta Win32 e Manutenção na porta Darwin.  
KO Myung-Hun - Porta OS/2.  
Jean-Baptiste Kempf - Gerente  
Markus Kuespert - Porta BeOS do DVD ioctls  
Pascal Levesque - Porta QNX.  
Steve Lhomme - Melhorias em win32.  
Christophe Massiot - Ex gerente.  
Steven M. Schultz - Porta BSD/OS.  
Alex Strelnikov - Porta OS/2.  
German Tischler - Patch de entrada FreeBSD DVD.  
Gildas Bazin - Manutenções diversas na porta Win32.  

<h3> 3 - Evolução do sistema </h3>

O projeto VideoLan foi iniciado na universidade École Centrale Paris a qual relicenciou a VLC sobre a licensa GPLv2 em fevereiro de 2001. Desde então, o VLC obteve mais de dois bilhões de downloads. Porém o software teve seu início como um projeto acadêmico em 1996 e como já citado anteriormente, VLC costumava significar VideoLan Client quando a aplicação se resumia a um software puramente cliente. Mas como a aplicação já não é mais exclusivamente um cliente seu nome original não se aplica mais. A intenção consistia em um cliente e um servidor para realizar streaming de vídeo através de um satelite para uso no campus da universidade em Paris.

O software foi reescrito completamente em 1998, e foi lançado sobre a licença GNU General Public License no dia 1 de fevereiro de 2001, autorizado pela chefia da École Centrale Paris. A funcionalidade servidora da aplicação, VLS (Video Lan Server) foi praticamente toda absorvida pelo VLC e sua independência foi descontinuada. Portanto o nome da aplicação foi alterado para VLC media player, pois não existia mais uma extrutura de cliente servidor.

Em 2007 por motivos de incompatibilidade de licensas, os líderes do projeto decidiram por não adotar a recém lançada licensa GPLv3 (General Public License version 3). Após 13 anos de desenvolvimento, a versão 1.0.0 do VLC media player foi lançada no dia 7 de julho de 2009. Já a integração com os dispositivos móveis com sistema operacional Android, tiveram seus trabalhos iniciados em em 2010 e a partir do ano de 2011 já se fazia disponível para download na Google Play para tais smartphones. Já a integração do VLC media player com os aparelhos da Apple de sistema operacional iOS, teve a responsabilidade transferida para uma empresa chamada Applidium, que ficou responsável por compatibilizar o software para tais smartphones. Ainda sobre a GPLv2 os trabalhos foram concluídos e aceitos na Apple Store no mês de setembro de 2010. Entretanto em janeiro de 2011, após a reclamação formal de um desenvolvedor contribuidor do VLC Rémi Denis-Courmont a respeito de conflitos relacionados às politicas de licensiamento entre a GPLv2 e as políticas da Apple Store, o aplicativo foi retirado da Apple Store pela própria Apple. Consequentemente os autores do VLC, começaram os processos de relicensiamento do software em outubro de 2011 passando de GPLv2 para LGPLv2 (GNU Lesser General Public License) para alcançar melhor compatibilidade de licença perante a Apple. Foi então em julho de 2013 que aplicação VLC pode submeter novamente o software na iOS Apple Store sobre a Mozilla Public License.

A versão 2.0.0 do VLC media player foi lançada em 18 de fevereiro de 2012, uma versão para a Windows Store foi lançada em 13 de março de 2014. Suporte para Windows RT, Windows Phone e Xbox One foram posteriormente adicionadas ao software. Em 2016 a aplicação já ocupa a terceira posição no ranking em [SourceForge.net](https://sourceforge.net/) de softwares mais baixados, posição que ocupa até hoje com a impressionante marca de mais de dois bilhões de downloads.

<h3> 4 - Frameworks, ferramentas e LPs </h3>

<h3> 5 - Documentação da arquitetura </h3>
