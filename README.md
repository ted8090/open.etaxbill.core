# Open eTaxBill for .Net Core

현재 .net core version으로 upgrade 중 입니다.

## Engine: 국세청 전자세금계산서 연동 서비스 엔진 

처리 하는 엔진 서비스들은 총 6가지로 구성 됩니다.

> collector: 전자 세금계산서를 작성 후 데이터베이스에 저장 하게 됩니다. 엑셀 파일을 업로드 하거나, ERP 시스템과 연동하여 다량의 세금계산서를 처리 합니다.

> signer: 매출자의 공인인증서로 서명하여, 발송 전 단계의 암호화된 전자세금계산서를 작성 합니다.

> reporter: 국세청에 전자세금계산서를 발송 합니다

> reponsor: 국세청으로 부터 처리 결과를 수신 받아서 내부 데이터베이스 저장 합니다.

> mailer: ASP 사업자와 매입자에게 전자세금계산서를 메일로 발송 합니다.

> provider: 타 ASP 사업자가 보내온 메일을 파싱하여 매입 전자세금계산서를 내부 데이터베이스에 저장 합니다.


## Channel: 전자세금계산 서버 호출용 채널 라이브러리

Open-eTaxBill의 6가지 서비스들을 각각 호출하는 WCF Channel 입니다.


## Certifier: 전자세금계산서 인증 프로그램

> [한국인터넷진흥원](https://www.taxcerti.or.kr/etax/)의 인증 절차를 통과 하기 위한 인증용 프로그램 입니다.

> 인증 순서와 맞춰서 메뉴 구성이 되어 있으니 그대로 따라가기 하시면 인증을 통과 할 수 있습니다.

