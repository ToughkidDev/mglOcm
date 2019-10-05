# mglOcm
rom file loader for 1chipMSX(KdL firmware machine) 


mglOCM is a MSX ROM loader for the  "KdL firmware's OneChip MSX"
 that allows you to run msx rom cartridge images (like Konami-SCC, ASCII-8 and ASCII-16, 8, 16, 32k, linear rom files)
 on your device without setting any DIP switches or mapper patches.

Rom Loader for 1Chip MSX - mglOCM v2.0370b (release date 2019/04/12)

v2.0370b :

ABOUT

	- This is the loader application that support to execute megarom cartridge images
	like Konami-SCC, Ascii-8 and Ascii-16 all mappers for 1Chip-MSX(OCM).

	- mglOcm is only for 1chip-MSX compatible loader which loads MSX-Rom image file
	needless to change any DIP switches and any mapper patches.

	- This is possible because mglOcm use 1chipMSX's hardware mapper controller, if you using mglOcm in
	load to rom image will complete supports ASCII8 and ASCII16 mappers
	and this executed megarom images perfectly.

SPECIFICATIONS
		- full MSX-DOS2 support
		- Konami Mapper with SCC
		- ASCII 8 kB Mapper
		- ASCII 16 kB Mapper
		- 2 romimages load to OCM's internal memory slots.

USAGE
		- MSXDOS2 must be loaded to run mglOcm.com
		- Youtube Video Link 
		- https://www.youtube.com/watch?v=oNPzevBzs64&list=PLlD0W14KLTkpq5dnONr_U6fAUWuyGliEw&index=80

Examples:
		- a:\roms> mglOcm gradius2.rom
		- a:\roms> mglOcm bublbobl.rom

...And more some command line options are as below.

		- /o = execute on Konami Classic Mapper
		- /s =    on Konami-SCC Mapper
		- /8 =    on Ascii-8 Mapper
		- /f =    on Ascii16 Mapper
		- /l =    on Linear  Mapper
		- /r = execute with alternative method
		- /t = Z80b 5.37MHz V9958 Fast mode
		- /k = Konami 2nd Cartridge secret option
		- /j = set Japanese keyboard layout
		- /d = back to DOS after loading

REQUIREMENTS
		- MSX-DOS2, KdL firmware of v3.1 and over.

CONTACT
		- "mglOcm" is written by ToughkidCST
		- toughkiddev@gmail.com







-------------------------
Korean 


- 개요 -  

-  mgOCM은 2006년도에 발매된 1ChipMSX(이하 OCM)을 기반으로 만들어진 OCM전용 메가롬파일 실행기입니다. 
   
   	1. mglOCM은 OCM을 전용으로 만들어진 최초의 메가롬파일 실행기로서 
	   OCM및 그외 OCMC와, 재믹스네오등, OCM을 기반으로 만들어진 MSX와 모두 호환됩니다.
      	   OCM에 대한 자세한 내용은 http://en.wikipedia.org/wiki/1chipMSX 

   	2. mglOCM의 특징 
     	   지금까지 메가롬로더로 사용되고 있는 로더들은 일반 MSX규격의 하드웨어에서 
	   범용적으로 실행될 수 있도록 만들어져 다양한 규격의 메가롬파일을 지원하는데 있어 한계를 보여 왔습니다. 
	   실례로 일반적인 메가롬파일을 지원하는 일련의 하드웨어들, 
	   SCC-I, MMC/SD, ESE-SCC, 메가플래시, 재미나 메가램팩등의 하드웨어들이 
	   코나미매퍼 방식으로 제작되어 있어, 그 외의 ASCII8, ASCII16등 여타 방식의 메가롬게임을 
	   지원하기 위해서는 코나미매퍼방식으로 프로그램에 변형을 가해 실행이 되도록 해야했습니다. 
	   문제는 파일의 이런 처리 이후 변형 및 파괴된 프로그램의 오동작등으로 인해 
	   호환성이 떨어지고,  또한  이런 문제를 해결하기 위해 나타난 다양한 방법들이, 
	   사용자들의 불편함을 가중시켜  게임을 즐기는데 있어 
	   접근성을 방해하는 요소로 작용했습니다. 

   	3. mglOCM은 게임롬파일에 패치등의 변형을  가하지 않고, 
  	   OCM에 내장된 하드웨어 매퍼를 사용하여, 게임롬파일의 실행 안정성을 극대화하고, 
  	   게임의 호환성을 확보했다는데에 그 의미가 있다고 하겠습니다.
  	   따라서 거의 대부분의 롬 게임은 그 어떤 파일의 변형 파괴나 OCM딥스위치의 변환없이 실행이 가능합니다. 

- 사용방법     
  mglocm.com [filename.rom] /opts

		mglOCM은 롬팩을 MSX에 삽입하듯,  사용하기 간단하게 만드는 것을 중요하게 생각하므로, 
		수많은 옵션들을 피하고 게임실행에 필요한 최소한의 것들만 사용하도록 하였습니다. 

		1. mglocm.com [filename.rom] 
		   기본적인 사용방법은 도스프롬프트에서 mglocm과 파일이름을 입력하는 것 뿐입니다. 
		   mglOcm은 실행되는 순간 짧은 시간을 통해 롬파일 방식을 파악하고 실행하도록 합니다. 
		   전반적으로 이 방법은 대부분의 게임을 실행하는데에 문제가 없는 방법입니다. 

			 예) mglocm gradius.rom  

		2. mglocm.com  [filename.rom] /opt
		   그럼에도 불구하고 다양한 매퍼방식을 지원하기 위해 필요한 최소한의 옵션을 
		   사용하실 수 있습니다 .
		
- 실행 옵션들 

		- /g - 만일 1번과 같은 방법으로 게임이 실행되지 않으면, /g 옵션을 사용하면
			게임파일을 분석해 정확한 매퍼와 실행방법을 알려줍니다. 
			거의 대부분의 게임은 이를 통해 실행 가능합니다. 

		- /r - (execute with alternative method)
   			일반적인 실행에 문제가 있는 몇몇 게임들에 대해 다른 방법의 실행방법으로  
   			게임을 구동하여 좀더 안정성을 강화합니다. 

		- /t - Z-80b CPU의 5.37MHz 파나소닉 터보 모드로 게임을 고속 실행합니다. 

		- /8 - ASCII8  방식의 매퍼를 사용하는 메가롬 게임을 실행합니다. 
			'/g'옵션을 통해 ASCII8방식인지 파악하실 수 있습니다. 

		- /f - ASCII16 방식의 매퍼를 사용하는 메가롬 게임을 실행합니다. 
			'/g'옵션을 통해 ASCII8방식인지 파악하실 수 있습니다. 

		- /d - 사용자의 필요에 따라 로딩후 도스로 돌아오는 옵션이 필요할 수 있습니다. 
			이를 위해 사용하십시요. 

		- /k - 코나미의 숨겨진 카트릿지 합성 비기를 사용할 수 있게 됩니다.
			이 옵션을 통해 MSX 카트리지 슬롯2에 추가로 카트리지를 삽입한 것과 같은 효과가 발생합니다. 
 	
		---------------------------------------------------------------------------
		
		'/k' -  "코나미10배로 즐기는 카트리지' 삽입
			'/k:keyword' - keyword에 해당하는  카트리지를 슬롯2에 삽입
			 	
	 	예) mglocm gradius.rom /k:twinbee
			그라디우스를 실행하고 슬롯2에 트윈비 카트리지를 삽입. 


- 코나미 합성비기가 발생하는 각 키워드는 다음과 같습니다. 

		- "kungfu",   이아쿵후
		- "kungfu2",  이아쿵후 황제의 역습
		- "kmare",    마성전설 
		- "twinbee",  트윈비
		- "gradius",  그라디우스
		- "mong",     몽대륙
		- "vampire",  악마성드라큘라
		- "kingkong", 킹콩
		- "qbert",    큐버트
		- "hinotori", 불새
		- "goemon",   간바레 고에몽
		- "galious",  마성전설2 갈리오우스의 미궁
		- "mgear",    메탈기어
		- "gradius2", 그라디우스2
		- "f1spirit", F1 스피리트
		- "usas",     우사스
		- "salamand", 사라만다. 

			     
- 코나미롬팩에 한해서 멀티롬 로딩이 지원됩니다.
   	이 기능을 통하여 카트릿지슬롯1번, 2번에 동시에 다른 게임을 삽입한 것과 같은 효과를 얻으실 수 있습니다. 	
   		"코나미 신10배로 즐기는 카트리지"나, 코나미 게임 합성등의 기능으로 사용하실 수 있습니다. 
   		    
  	1. 사용법 
    	mglocm.com [file1.rom] [file2.rom] 

  	2. ex)    mglOcm.com gradius1.rom twinbee.rom 
    	슬롯1번에 gradius1 삽입효과,  슬롯2번에 twinbee 삽입효과

- 사용환경 
 	KDL의 MSX2+ 기반 펌웨어 3.1이상.  모든 OCM환경내 MSX-DOS2이상. 

- 주의사항 
	
	 	1. mglOCM은 여러가지의 이유로 특정 상황을 지원하기 위해 
    		** 패치 변형된 롬파일에 대해서는 정상적인 실행을 보장하지 않습니다. 
   		원본 롬파일을 사용해 주시기 바랍니다. 
 
  		2. 롬파일중 롬팩내에 s-ram과 같이 내부 밧데리 백업기능을 내장하고 있었거나, 
     		그 외 특수 칩을 사용해 특수기능이 내장된 롬팩게임의 구동은 보장하지 않습니다. 


		
