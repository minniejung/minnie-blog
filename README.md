# minnie-blog

## 31/01/2025 - THE FIRST DAY

```
[OT]
    
  - 전반적인 채용시장
  - 커리큘럼 소개
```

## 03/02/2025 - BITCOIN & BLOCKCHAIN 
```
[Cypherpunk's Manifesto (1993, Eric Hughes)]

  - 프라이버시는 기본적인 인간의 권리
    * 개인이 자신의 정보를 자유롭게 통제할 수 있어야 한다.
    * 감시 없는 자유로운 사회를 위해 필수적이다.
   
  - 정부와 기업의 감시 위험
    * 온라인 활동이 추적, 기록, 분석되면서 개인의 자유가 침해된다.
    * 중앙집중화된 데이터 관리 구조는 위험하다.

  - 해결책은 암호화 기술
    * 법이나 제도가 아니라 강력한 암호화 기술(Encryption) 만이 프라이버시를 보장할 수 있다.
    * 정보는 암호학을 통해 보호되어야 하며, 이는 누구나 사용할 수 있어야 한다.

  - 탈중앙화가 핵심
    * 중앙기관을 신뢰할 필요 없는 P2P(개인 간) 시스템을 구축해야 한다.
    * 개인이 자신의 데이터를 직접 소유하고 관리해야 한다.

  - "Cypherpunks write code"
    * 말이 아니라 직접 기술을 만들어야 한다.
    * PGP 암호화, Tor 네트워크, 블록체인(Bitcoin) 같은 도구가 핵심이다.
   
  - 영향 및 유산
    * 비트코인과 블록체인 탄생에 기여 (검열 없는 탈중앙 금융)
    * 암호화된 커뮤니케이션 도구 발전 (PGP, Signal, Tor)
    * Web3, 프라이버시 기술, 디지털 권리 운동의 기반 철학 제공
```

```
[Bitcoin]

  - 세계 금융 위기가 발생한 2008년 10월 31일. 사이퍼 펑크 메일링 리스트에 "Bitcoin P2P e-cash paper" 라는 이름의 메일이 등장
  - 9쪽 짜리의 비트코인 백서("Bitcoin: A Peer-to-Peer Electronic Cash System")와 비트코인이 세상에 처음으로 등장
```

```
[Pizza day (2010. 5. 22)]

    - 라스즐로 핸예츠(Laszlo Hanyecz)라는 프로그래머가 비트코인을 이용해 처음으로 피자 2판을 구매
    - 비트코인을 사용한 최초의 실물 거래
    - 비트코인이 화폐로써 기능을 할 수 있음을 인식하는 계기가 됨
```

```     
[Genesis Block]

  - 2009년 1월. 첫 번째 블록(제네시스 블록) 채굴을 시작으로 소스 코드 공개와 함께 비트코인 등장

  - 중앙화 금융 시스템에 대한 비판
    * 중앙은행과 정부가 주도하는 중앙화된 금융 시스템의 불안정성과 문제점을 비판
    * 금융위기 당시 은행들이 무분별한 투자를 했음에도 불구, 실패의 책임을 국민이 떠안아야 한다는 구조에 강한 문제의식을 가짐

  - 탈 중앙화 금융의 대안 제시
    * 비트코인은 중앙 기관 없이 작동하는 탈중앙화 디지털 화폐로 설계되었으며, 이를 통해 기존 금융 시스템의 문제를 극복하고자 함
    * 메시지를 통해 비트코인의 철학(탈중앙화, 신뢰 없는 시스템)을 상징적으로 드러냄

  - 역사적 맥락을 기록
    * 제네시스 블록에 메시지를 포함함으로써, 비트코인이 어떤 문제를 해결하려는 목적으로 탄생했는지를 명확히 전달
    * 비트코인의 기원이 글로벌 금융위기의 한복판에서 비롯되었음을 명시적으로 기록
```   

## 04/02/2025 (1) - HASH
```
Q. 해시(Hash)란?
A. 데이터를 압축하고 고정된 크기의 출력값. 주로 데이터의 무결성을 확인하거나 암호학적 보안을 제공하는 데 사용.

[타임 스탬프 해시 생성 과정]
  데아터 준비 -> 데이터를 고정된 길이의 해시 값으로 변환 -> 해시 값을 타임스탬프 기관(TSA, Timestamp Authority)에 제출
  -> TSA가 사용자가 제출한 해시 값 + 타임 스탬프 + 서명을 추가한 결과를 반환 -> 데이터 검증
```

```
Q. 해시 함수의 특징?
A. 입력 데이터의 크기와 관계없이 고정된 길이 (e.g. SHA-256는 256비트(32바이트))
   서로 다른 입력 데이터가 동일한 해시 값을 가지는 가능성은 극히 낮음
   역으로 계산하는 것은 불가능
   현대 컴퓨터에서 빠른 계산이 가능
   현재까지는 실질적인 공격/충돌 생성이 매우 어려움
```

```
Q. 해시 함수의 활용?
A. 블록체인 - 암호화폐의 데이터 무결정을 보장하고 체인 연결하는 데 사용
   디지털 서명 - 데이터 인증 및 무결성 확인
   암호화 저장 - 비밂번호 및 중요한 데이터를 안전하게 저장
   데이터 검증 - 파일 다운로드 및 전송 중 데이터 손상 여부 확인 가능
```

```
Q. SHA-256 알고리즘 작동 과정?
A. 입력 데이터 준비 (512비트 블록으로 처리 됨)
   -> 부족한 비트를 채우기 위해 패딩 추가 (1을 추가 후 데이터 길이가 512비트의 배수가 될때까지 0을 추가, 그리고 길이정보 추가)
   -> SHA-256의 8개의 32비트 초기 해시 값과 함께 라운드 연산을 통해 최종 해시 값 출력
```

```
Q. 블록 해시 값 생성 인자는?
A. Version, Prev block hash, Merkle root, Timestamp, Difficulty target, Nonce

PoW 작업 증명을 위해 채굴자들은 Nonce랑 Timastamp를 MerKle root를 계속해서 수정해 가며 퍼즐을 풀어야 함
e.g. 000000000000000000015ac6f0b07acb480cff6a6fd389350398cbe8455994a9
     블록 해쉬의 0의 개수가 많을 수록 난이도가 높음
```

```
[대칭키 암호화]

  - 대칭키는 암호화와 복호화에 모두 사용됨
  - 평문 데이터를 입력받아 비밀 키를 사용하여 암호문으로 변환
  - 암호문은 안전하지 않은 네트워크를 통해 수신자에게 전송 됨
  - 비밀 키를 아는 사람만 암호문을 복호화할 수 있습니다.
  - 수신자가 동일한 비밀 키를 사용하여 암호문을 평문으로 복호화합니다.

    e.g. 개발팀 환경셋팅, 금고 열쇠, 공용 비밀번호
```

```
[비대칭키 암호화]

  - 공개키(PublicKey) 와 개인키(비밀키, PrivateKey) 를 한 쌍으로 사용되는 암호화 방식
  - 개인키 생성 후, 개인 키로부터 공개 키를 생성 (개인 키에서 공개 키는 유추 가능하나 반대로는 불가)

    e.g. 디지털 서명(트랜잭션 서명 등)

[공개 키로 암호화 (Encryption using Public Key)]

  - 공개 키로 암호화 할 시, 대항 데이터를 복호화 할 수 있는 사람은 오직 해당 개인 키를 가진 사용자 뿐
  - 블록체인에서는 데이터의 기밀성을 보장하기 위해 공개 키로 암호화하는 방식은 자주 사용되지는 않음
  - 동작원리 : 송신자가 수신자의 공개 키로 데이터를 암호화 -> 수신자는 자신의 개인키로 데이터를 복호화

[개인 키로 암호화 (Encryption/Signing using Private Key)]

  - 디지털 서명
      1. 송신자가 자신의 개인 키로 데이터를 서명 ->
      2. 서명된 데이터는 수신자에게 전송 ->
      3. 수신자는 서명된 데이터와 발신자의 공개 키를 사용해 서명을 검증 ->
      4. 이를 통해 데이터가 발신자로부터 생성되었고 중간에 변경되지 않았음을 증명
```

## 04/02/2025 (2) - DIGITAL SIGNATURE
```
[디지털 서명]

  - 서명의 역할은 문서의 진위성과 무결성을 보증하는 것
  - 디지털 서명은 개인 키(Private Key)를 사용하여 생성
  - 개인 키로 데이터를 서명함으로써, 서명의 주체가 ‘나’라는 것을 인증할 수 있으며, 이 데이터가 변조되지 않았음을 증명

  - 디지털 서명된 데이터를 수신한 사용자는 공개 키(Public Key)를 사용해 서명을 검증하며 서명과 데이터가 일치하는지를 확인
      1. 데이터의 무결성 : 데이터가 전송 중 변조되지 않았는지
      2. 진위성 확인 : 데이터를 서명한 사람이 신뢰할 수 있는 발신자인지
      3. 부인 방지 : 송신자의 개인키가 안전하게 보관되었다는 전제하에, 서명 생성 후에는 이 서명이 송신자에 의해 서명되었다는 사실을 부정할 수 없음

[디지털 서명의 장점]

  - 보안성: 개인 키가 노출되지 않는 한, 다른 사용자가 서명을 위조할 수 없음
  - 무결성 보장: 트랜잭션 데이터가 변조될 경우, 서명이 유효하지 않게 됨
  - 부인 방지: 송신자는 자신이 해당 트랜잭션에 서명했음을 부정할 수 없음
  - 신뢰 기반 탈중앙화: 디지털 서명은 중앙 기관 없이도 트랜잭션의 신뢰성을 보장

```

```
[타임스탬프에서의 디지털 서명의 사용 목적]

  - 무결성 증명 : 데이터가 특정 시점 이후로 변경되지 않았음을 보장, 디지털 서명을 통해 변조되지 않았음을 검증
  - 시간 인증 :  데이터가 특정 시간에 존재했음을 증명, 타임스탬프 인증 기관이 디지털 서명을 통해 해당 시간에 데이터를 인증
  - 신뢰 제공 : 디지털 서명은 인증 기관의 신뢰를 바탕으로 데이터의 진위를 보증
```

```
[비트코인에서 디지털 서명의 역할]

  - 트랜잭션 무결성 증명 : 트랜잭션 데이터가 변경되지 않았음을 보장
  - 소유권 증명 : 트랜잭션을 생성한 사용자가 해당 비트코인의 소유자임을 증명
  - 탈중앙화된 검증 : 디지털 서명을 검증하여 트랜잭션의 유효성을 확인, 중앙 기관 없이 신뢰를 유지할 수 있도록 함
```
