﻿# 대한민국 행정동 경계(admdongkor)

- 저작권 관련 사항은 본 문서의 끝부분에 기술하였으니 참고하시기 바랍니다.  

## 대한민국 행정동 경계 파일입니다.
- 통계청 통계지리정보서비스에서 제공하는 행정동 경계 파일을 바탕으로, 행정동 변경 이력을 수정하여 반영한 파일입니다.
- geojson 형식이며, 좌표계는 WGS84 (EPSG:4326) 입니다.
- geojson 및 csv 파일 인코딩 형식은 UTF-8입니다.
- topology 정합성을 검토하였습니다.(폴리곤 경계끼리 잘 맞습니다) 
- 속성의 adm_cd 는 통계청에서 사용하는 7자리의 [한국행정구역분류코드]입니다.
- 속성의 adm_cd2 는 행정안전부 사용하는 10자리의 [행정기관코드]입니다.(2018.07.24 업데이트 파일부터 적용)
- 속성의 adm_nm 은 통계청에서 사용하는 전국 행정동 이름입니다.
- 일부 지역들이 실제 행정동 경계와 잘 맞지 않습니다. 지속적인 수정이 필요합니다.
- 최신 버젼만 업로드하지 않고 변경 이력별로 지속적으로 남길 예정입니다.
- 앞으로의 변화를 수정할 경우 'for update' 폴더 안의 파일을 fork하여 수정한 후 수정내역.txt와 함께 pull request 해 주시면 검토 후 master branch에 반영하겠습니다.
  - 수정과 업로드는, 폴리곤을 단순화시키지 않은 가장 상세한 버젼으로 올려주시기 바랍니다.

## 통계청 마이크로데이터서비스(MDIS) 인구이동 데이터용 행정동 경계 중심점
- [통계청MDIS인구용_행정경계중심점] 폴더에는 통게청 MDIS 의 인구이동 데이터와 매칭시킬 수 있는 행정 경계 중심점 파일이 있습니다.
- 행정안전부에서 사용하는 10자리 코드 기준입니다. 좌표계는 UTMK(EPSG:5179, KOREA 2000 Unified CS)
- 최신 자료인 2001~2020년에 존재하는 모든 출장소, 읍면동, 시군구, 시도 중심점이 있습니다. 출장소는 위치를 별도로 찾아서 입력해두었습니다.
- 서울특별시 같은 경우 1100000000으로, 서울 종로구 같은 경우 1111000000 등 10자리로 맞춰 놓았습니다.
- 과거 행정구역 경계 파일에서 중심점을 추출하고 일부 수작업으로 이동시켰습니다. 
- 청원군처럼 도너츠 형상으로 되어 있는 곳은 임의로 옮겼지만, 위치가 마음에 안 들 수도 있습니다. 필요한 부분은 수정해서 사용하시면 됩니다.



## 파일 버젼

- ver20210101
  - 2020년 10월 26일 인천광역시 연수구 송도4동이 송도4동과 송도5동으로 분할 되었습니다.
  - 2020년 11월 1일 울산광역시 울주군 삼남면이 삼남읍으로 승격되었습니다.
  - 2020년 12월 1일 경기도 광주시 경안동이 경안동과 쌍령동으로 분할,
  - 2020년 12월 1일 경기도 광주시 송정동이 송정동과 탄벌동으로 분할,
  - 2020년 12월 1일 경기도 광주시 광남동이 폐지되고 광남1동과 광남2동으로 분할되면서 신설되었습니다.
  - 2021년 1월 1일 강원도 양구군 남면이 국토정중앙면으로 명칭변경되었습니다.
  - 2021년 1월 1일 경상북도 구미시 산동면이 산동읍으로 승격,
  - 2021년 1월 1일 경상북도 구미시 비산동과 공단1동이 비산동으로 통합,
  - 2021년 1월 1일 경상북도 구미시 공단2동이 공단동으로 명칭변경되었습니다.
  - 2021년 1월 1일 경상북도 군위군 고로면이 삼국유사면으로 명칭변경되었습니다.

- ver20201001
  - 2020년 7월 6일 대구광역시 동구 안심3.4동이 안심3동, 안심4동, 혁신동으로 분할되었습니다.
  - 2020년 7월 6일 대구광역시 동구 불로봉무동과 지저동 사이의 경계가 조정, 신암1동과 신암4동 사이의 경계가 조정되었습니다.
  - 2020년 7월 15일 세종특별자치시 연기면 지역 일부가 도담동으로 편입되었습니다.(경계조정)
  - 2020년 7월 15일 세종특별자치시 금남면과 연동면 지역 일부가 소담동으로 편입되었습니다.(경계조정)
  - 2020년 7월 20일 경상북도 구미시 행정동 간의 경계가 일부 조정되었습니다.(경계조정)
  - 2020년 7월 27일 광주광역시 북구 건국동이 건국동과 신용동으로 분할,  
  - 2020년 8월 14일 세종특별차지시 새롬동이 새롬동과 다정동으로 분할되었습니다. 


- ver20200701
  - 2020년 4월 20일 경기도 하남시 감북동이 감북동과 감일동으로 분할되었습니다.
  - 세종시 일부 토폴로지 오류를 수정하였습니다.


- ver20200401 + 20200515
  - 2020년 1월 6일 경기도 의정부시 의정부1동과 의정부3동이 의정부1동으로 통합,
  - 2020년 1월 13일 경기도 의정부시 송산2동이 송산2동과 송산3동으로 분할,
  - 2020년 1월 20일 경기도 용인시 기흥구 영덕동이 영덕1동과 영덕2동으로 분할,
  - 2020년 1월 20일 경기도 용인시 기흥구 상갈동이 상갈동과 보라동으로 분할,
  - 2020년 1월 20일 경기도 용인시 기흥구 동백동이 동백1동, 동백2동, 동백3동으로 분할,
  - 대구광역시 달성군 현풍읍의 통계청 코드 미반영 오류를 정정,
  - 전라북도 김제시 만경읍과 성덕면 사이의 토폴로지 오류를 수정하였습니다.
  - 통계청의 재수정으로 경상남도 사천시 벌룡동의 이름이 벌용동으로 정정, 시흥시 장곡동 관할구역 경계가 일부 변경되었습니다.


- ver20200101
  - 2020년 1월 1일에 다수의 행정동이 변경되었습니다.
  - 서울특별시 구로구 오류2동이 오류2동과 항동으로 분할, 
  - 부산광역시 금정구 장전2동, 장전3동이 장전2동으로 통합,
  - 경상남도 창원시 마산합포구 교방동과 노산동이 교방동으로 통합, 
  - 경상남도 창원시 진해구 중앙동, 태평동, 충무동이 충무동으로 통합, 
  - 전라남도 화순군 북면과 남면이 각각 백아면과 사평면으로 이름 변경,
  - 경상북도 경산시 압량면이 압량읍으로 승격,
  - 경상북도 상주시 사벌면이 사벌국면으로 이름 변경되었습니다.


- ver20191231
  - 2019년 10월 21일 경기도 화성시 동탄6동이 동탄6동과 동탄8동으로 분할되었습니다.
  - 2019년 11월 4일 인천광역시 서구 당하동이 당하동과 마전동으로 분할되었습니다.
  - 통계청 2020년 1월 1일 공지파일에 2019년 12월 31일과 2020년 1월 1일을 구분해 놓았으므로 이 자료에서도 동일하게 구분하였습니다.


- ver20191001
  - 2019년 9월 23일 경기도 김포시 구래동이 구래동과 마산동으로 분할되었습니다.
  - 2019년 9월 30일 경기도 평택시 비전2동이 비전2동과 용이동으로 분할되었습니다.
  - 2019년 10월 1일 전라북도 전주시 덕진구 동산동의 이름이 여의동으로 변경되었습니다.
  - 통계청에서 변경이력을 1년에 정기적으로 네 번(1.1, 4.1, 7.1, 10.1) 공지합니다. 앞으로 업데이트는 공지한 날짜의 변경분까지 반영할 예정입니다.


- ver20190908
  - 2019년 4월 15일 경기도 수원시 영통구 태장동이 망포1동과 망포2동으로 분할되었습니다.
  - 2019년 7월 1일 경기도 화성시 동탄6동이 동탄6동과 7동으로 분할되었습니다.
  - 2019년 7월 1일 충청북도 진천군 덕산면이 덕산읍으로 승격되었습니다.
  - 2019년 7월 1일 경기도 부천시의 행정동이 10개 행정동으로 통폐합되었습니다.
  - 2019년 7월 1일까지 변경된 행정동의 adm_cd 속성에는 새로 부여된 7자리코드를 적었습니다.
  - 2019년 7월 1일까지 변경된 행정동의 adm_cd2 속성에는 모두 변경된 10자리 코드로 수정했습니다.  


- ver20190403
  - 2019년 1월 1일 인천광역시 연수구 송도2동이 송도2동과 송도 4동으로 분할되었습니다.
  - 2019년 2월 19일 전라남도 담양군 남면의 이름이 가사문학면으로 변경되었습니다. (경계 불변)
  - 2019년 3월 1일 경상북도 청송군 부동면의 이름이 주왕산면으로 변경되었습니다. (경계 불변)
  - 2019년 4월 1일까지 변경된 행정동의 adm_cd 속성에는 새로 부여된 7자리코드를 적었습니다.
  - 2019년 4월 1일까지 변경된 행정동의 adm_cd2 속성에는 모두 변경된 10자리 코드로 수정했습니다.  
  - 서울특별시 마포구 합정동과 서교동의 꼬인 경계를 수정하였습니다.


- ver20181106
  - 2018년 9월 27일 경기도 의정부시 가능1동의 이름이 가능동으로 명칭변경되었습니다. (경계 불변)
  - 2018년 10월 1일 부산광역시 금정구 금사동의 이름이 금사회동동으로 명칭변경되었습니다. (경계 불변)
  - 2018년 10월 8일 경기도 시흥시 정왕4동이 정왕4동과 배곧동으로 분할되었습니다.
  - 2018년 11월 1일 대구광역시 달성군 옥포면과 현풍면이 옥포읍과 현풍읍으로 승격되었습니다. (경계 불변)
  - 2018년 11월 5일 인천광역시 남동구 장수서창동이 장수서창동과 서창2동으로 분할되었습니다.
  - 2018년 10월 1일까지 변경된 행정동의 adm_cd 속성에는 새로 부여된 7자리코드를 적었으며, 그 이후 변경된 행정동의 마지막 두자리는 알파벳으로 처리하였습니다.
  - 2018년 11월 5일까지 변경된 행정동의 adm_cd2 속성에는 모두 변경된 10자리 코드로 수정했습니다.  

- ver20180724
  - 2018년 7월 23일까지 변경된 모든 행정동에 10자리 행정기관코드를 추가하였습니다. (adm_cd2 필드 참고)
  - 2018년 7월 1일 경기도 고양시 덕양구 신도동이 삼송동으로 명칭 변경되었습니다. (경계 불변)
  - 2018년 7월 1일 인천광역시 서구 행정동 명칭이 5건 변경되었습니다. (경계 불변)
  - 2018년 7월 1일 전라북도 전주시 완산구 효자4동이 효자4동,효자5동,덕진구 혁신동으로 3분할 되었습니다.
  - 2018년 7월 1일 인천광역시 남구가 인천광역시 미추홀구로 명칭 변경 되었습니다. (경계 불변)
  - 2018년 7월 16일~23일에 세종특별자치시 보람동이 보람동, 대평동, 소담동으로 3분할 되었습니다.
  - 2018년 7월 1일까지 변경된 행정동은 새로 부여된 코드를 적었으며, 그 이후 변경된 행정동 코드의 마지막 두자리는 알파벳으로 처리하였습니다.
  

- ver20180401
  - 2018년 4월 1일 울산광역시 울주군 청량면이 청량읍으로 명칭 변경되었습니다. (경계 불변)
  - 2018.6.13 제7회 전국동시지방선거의 행정동 경계로 사용할 수 있습니다. 중앙선거관리위원회 홈페이지에서 청량면 -> 청량읍 변동분까지 반영된 것을 확인하였습니다.

- ver20180301
  - 2017년 12월 11일 경기도 용인시 처인구 모현면과 이동면이 모현읍과 이동읍으로 변경되었습니다. (경계 불변)
  - 2017년 12월 18일 경기도 남양주시 다산1동과 다산2동이 신설되면서 영역과 명칭이 세부적으로 조정되었습니다.
  - 2017년 12월 26일 경기도 수원시 영통구 영통1,2동이 조정되고 영통3동이 신설되었습니다.
  - 2018년 1월 1일 부산광역시 강서구 명지동이 명지1,2동으로 분동되었습니다.
  - 2018년 1월 1일 인천광역시 중구 영종동이 영종동과 영종1동으로 분동되었습니다.
  - 2018년 1월 22일 경기도 화성시 새솔동이 신설되고 동탄 4,5,6동이 조정되었습니다.
  - 2018년 3월 1일 대구광역시 달성군 유가읍이 유가면으로 변경되었습니다.
  - 2018년 1월 1일까지 변경된 행정동은 새로 부여된 코드를 적었으며, 그 이후 변경된 행정동 코드의 마지막 두자리는 알파벳으로 처리하였습니다.

- ver20171016
  - 2017년 8월 1일까지 변경된 행정동의 7자리 코드를 채워넣었습니다. 2017년 10월 1일에 통계분류포털에 업데이트 된 행정구역분류코드를 이용하였습니다.
  - 2017년 10월 16일 세종특별자치시 한솔동이 한솔동과 새롬동으로 나뉘었습니다.
  - 변경된 행정동의 코드의 마지막 두자리는 알파벳으로 처리하였습니다.(통계청관리 코드를 아직 알 수 없음)

- ver20170801
  - 2017년 7월 17일 경기도 안산시상록구와 안산시단원구의 일부 행정동의 명칭이 변경되었습니다. 원곡본동의 경우 원곡동과 신길동으로 나뉘었습니다.
  - 2017년 8월 1일 충청남도 홍성군 홍북면이 홍북읍으로 변경되었습니다.

- ver20170418
  - 2017년 4월 18일에 변경된 경기도 김포시 김포본동, 장기본동까지 반영되어 있습니다.
  - 2017년 5월 대통령선거에 사용가능한 버젼입니다.  
  - 중앙선거관리위원회에서 사용하는 행정동 이름과 매칭시킬 수 있는 csv를 동봉하였습니다.
  - 통계청 파일에서 수정한 경계(실제 행정구역도와 대조함, 행정구역 변경 이력과는 별개임)
    - 서울특별시 송파구 위례동, 경기도 성남시 수정구 위례동, 경기도 하남시 위례동의 경계 부근
    - 부산광역시 해운대구
    - 경기도 시흥시의 오이도 부근

- ver20160201
  - 2016년 2월 1일까지의 변경부분이 반영되어 있습니다.
  - 2016년 4월 국회의원 선거에 사용가능한 버젼입니다.
  - 중앙선거관리위원회에서 사용하는 행정동 이름과 매칭시킬 수 있는 csv를 동봉하였습니다.
    - 통계청 행정동과 선관위 행정동은 '제1동' 등에서 차이나는 것이 있습니다.
    - 선거구 획정에 따라 선관위 관할구역이 행정구와 일치하지 않는 경우가 있습니다(중앙선관위 선거통계시스템 FAQ참고). 해당 값들을 매칭시켰습니다.
    - 위의 두 경우는 csv의 '특이사항' 필드에 1로 표시하여 두었습니다.
  - 통계청 파일에서 수정한 경계(실제 행정구역도와 대조함, 행정구역 변경 이력과는 별개임)
    - 서울특별시 송파구 위례동, 경기도 성남시 수정구 위례동, 경기도 하남시 위례동의 경계 부근
    - 부산광역시 해운대구

- ver20121210
  - 2012년 12월 10일까지의 변경부분이 반영되어 있습니다.
  - 2012년 12월 대통령선거에 사용가능한 버젼입니다.



## 속성의 adm_cd
- 통계청에서 사용하는 7자리의 [한국행정구역분류코드]입니다.
- [2자리 시도]+[3자리 시군구]+[2자리 읍면동] 으로 이루어집니다.
  - 따라서,  코드의 특정 문자열들을 이용하여, dissolve로 병합하면 시도 경계나 시군구 경계 파일을 만들 수 있습니다.
  - dissolve 방법은 아래 mapshaper에 설명해 두었습니다.
- 행정동 경계가 변하면 행정동 이름이 그대로이더라도 코드가 변경됩니다.

## 속성의 adm_cd2
- 행정안전부(행정자치부, 안전행정부 등 이름이 바뀌어도 *행정*부)에서 사용하는 10자리의 행정기관코드입니다.
- [2자리 시도]+[3자리 시군구]+[3자리 읍면동]+[2자리 행정리] 로 이루어집니다.
  - 따라서,  코드의 특정 문자열들을 이용하여, dissolve로 병합하면 시도 경계나 시군구 경계 파일을 만들 수 있습니다.
  - 행정동 이외에 출장소에도 코드가 부여되어 있습니다.
- 행정동 경계가 변해도 행정동 이름이 그대로이면 코드가 변경되지 않습니다.

## 참고 : 행정동 관련 정보
- 2018년 8월 현재, 과거 행정동 경계 파일을 제공하는 곳은 통계청 통계지리정보서비스가 유일합니다.
  - https://sgis.kostat.go.kr/contents/shortcut/shortcut_05_02.jsp
  - 로그인 후 자료신청을 통해 받을 수 있습니다.
  - 2017년 5월 현재 1975~2015년 까지 받을 수 있습니다.
  - 2015년 버젼은 2015년 10월 1일의 행정구역 변경이력까지 반영된 파일입니다.
- 최근 업데이트 된 행정동 경계 파일은 국가공간정보포털에서도 다운받을 수 있습니다.
  - 경계 좌표의 해상도가 매우 자세합니다. 경계의 위상도 그럭저럭 어긋남 없이 잘 맞습니다.
  - 다만 데이터의 업데이트 시점이 다소 늦습니다. 2021년 1월에 업데이트 된 파일은 2020년 6월 버젼입니다.
- 선거 득표 등 특정한 시점의 이벤트를 행정동에 빠짐 없이 맵핑하려면 세세한 행정구역 변경 이력을 확인해야 합니다.
- 행정구역분류 코드 및 변경 이력은 1년에 4번, 분기별로 통계청에 업데이트 됩니다.
  - http://kssc.kostat.go.kr → 행정구역분류 → 자료실
  - 이 곳의 자료로 통계청의 [7자리 행정구역분류코드], 행자부의 [10자리 행정표준코드관리시스템 코드], [10자리 법정동 코드]를 매칭시킬 수 있습니다.
  - 이 곳의 자료에서 과거 행정구역 변경 이력을 알 수 있습니다.
  - 0번 시트에 행정동 코드에 대한 설명이 있습니다.
- 연중 지속적으로 이루어지는 행정구역 변경은 행정안전부 홈페이지에 게시됩니다.
  - http://www.mois.go.kr/frt/bbs/type001/commonSelectBoardList.do?bbsId=BBSMSTR_000000000052
  - [행정안전부 홈페이지](http://www.mois.go.kr/) → [업무안내 → 지방자치분권실 → 주민등록 및 인감] 게시판에서 ‘주민등록주소코드 변경내역’이라는 제목들로 올라온 글에 변경내용이 있습니다.
- 행정구역 코드 변경은 다음과 같이 이루어지는 것 '같습니다'
  - 7자리 코드는 동 통폐합이나 이름 변경시 새로 부여됩니다.
  - 10자리 코드는 통폐합 되더라도 과거의 동 이름이 살아있는한 해당 동의 코드는 그대로 유지됩니다.
- 통계청마이크로데이터서비스의 인구이동 데이터는 10자리 코드와 매칭됩니다. 단, 행정동 이외에도 출장소에 신고된 전입전출 데이터도 있으니 유의하시기 바랍니다.
- 행정동의 관할 법정동 지번과의 관계는 각 시의 조례에 지번까지 상세하게 나와있습니다. 
  - ex) 경기도 안산시 행정운영동의 설치 및 관할구역에 관한 조례

## 참고 : 선거 및 지도 관련 데이터
- 과거 선거 관련 데이터 원본은 [중앙선거관리위원회](http://nec.go.kr/portal/bbs/list/B0000341.do?menuNo=200029)에서 찾을 수 있습니다.
- [2017년 대선 시군구별 득표 지도](https://bl.ocks.org/vuski/raw/e29ed35cfdfb21ae01689c76f4aeea87/) 와 [2017년 대선 읍면동별 득표 지도](https://bl.ocks.org/vuski/raw/7e482f13ef2b2ec4c14bb3622f05c353/) 를 인터랙티브 버젼으로 볼 수 있습니다. 지역별 1~5위 득표지도, 후보별 득표지도, 2016년 총선과의 비교지도가 있고 총 14장입니다. 개략적 지도의 모습과 설명은 [여기](http://www.vw-lab.com/39)에서 확인할 수 있습니다. 시군구별 득표지도는 모바일 화면에 최적화 되어 있고, 읍면동별 득표지도는 pc 화면 비율(가로로 긴 화면)에 최적화 되어 있습니다. 읍면동 득표지도는 모바일에서 느려질 수 있습니다. 
- [ChangHee Lee 님의 repository](https://github.com/WWolf/korea-election)에 몇몇 과거 선거 데이터들과 관련 자료들이 정리되어 있습니다.
- [오마이뉴스 repository](https://github.com/OhmyNews/2017-Election)에도 2017년 대선 데이터과 분석 자료들이 올라와 있습니다.
- [southkorea 계정의 repository](https://github.com/southkorea/southkorea-maps)에는 2011년~2013년 지도 데이터들이 다양한 포맷으로 올라와 있습니다.


## 참고 : mapshaper
- mapshaper.org 에서 여러 가지 작업을 할 수 있습니다. 자세한 것은 다음의 링크를 참고하세요
  - https://github.com/mbloch/mapshaper/wiki
- 맵셰이퍼에서 가능한 작업들
  - 간단한 토폴로지 불일치 자동 수정
  - 웹 용으로 사용할 수 있도록 simplify 하여 용량 줄이기
  - topojson 으로 변경하여 용량 극소화 하기, 기타 다른 형식으로 변경 가능
  - dissolve 등의 명령 사용 가능
- 행정동을 시군구 경계로 병합하는 방법
  - mapshaper에서 import 후 오른쪽 위의 console 버튼을 눌러 콘솔창을 띄웁니다.
  - -info 명령어로 속성들이 들어와 있는지 확인합니다
  - each 'sgg_cd=adm_cd.substr(0,5)' 명령으로 시군구 코드를 추출해냅니다.
  - each 'sgg_nm=adm_nm.substr(0,adm_nm.lastIndexOf(" "))' 명령으로 시군구 이름을 추출합니다.
  - dissolve sgg_cd copy-fields=sgg_nm 명령으로 시군구 코드 기준으로 병합합니다. 동시에 시군구 이름은 복사해둡니다.
  - 모든 작업이 끝났으므로 Export 하면 됩니다.

## 저작권 관련
- 이 github에서 배포하는 행정동 경계 데이터는 통계청 통계지리정보서비스에 요청하여 받은 2010년과 2015년 경계를 바탕으로 수정한 것입니다.
  - 통계지리정보서비스(sgis.kostat.go.kr)에서는 '제공된 자료에 대한 출처를 반드시 명시'하라는 사항 이외에 별다른 저작권에 대한 사항이 나와 있지 않습니다.
  - 따라서, <공공데이터의 제공 및 이용 활성화에 관한 법률> 3조에 따른다고 해석하여 몇 가지 예외사항을 제외하고는 영리적 이용도 가능하다고 판단하고 있습니다.
- 그리고 원 시점(2010, 2015년)에서 수정을 가한 이 github의 자료 역시 별도의 추가적인 제한을 두지 않습니다.
  - 즉, 자유롭게 이용하시되 이용자의 판단하에 이  github의 주소(https://github.com/vuski/admdongkor)를 표시하여 주시길 권장합니다.
  - 이는 수정된 부분에 대한 저작권을 주장하기 위함이 아니라, 자료에 문제나 틀린 부분을 발견하는 사람이 있을 경우 이 곳을 찾아올 수 있도록 하기 위함입니다.
- 자료의 이용에 대한 책임은 어디까지나 이용자 본인에게 있습니다. 
  - 행정동 경계 중 이용 목적과 중요하게 관련된 부분이 있을 경우 위에 기술한 관련 정보를 통해 직접 경계를 확인하신 후 사용하시기 바랍니다.
