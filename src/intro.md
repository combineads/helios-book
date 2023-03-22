# Helios 소개

[Helios](https://github.com/Hyperion-BT/Helios)는 [Cardano](https://www.cardano.org) 블록체인을 위한 스마트 컨트랙트 작성을 위한 [DSL](./lang/index.md) (도메인 특화 언어)입니다.

[Helios 라이브러리](https://github.com/Hyperion-BT/Helios)는 자바스크립트로 작성되어 있으며 다음을 위한 [API](./api/index.md)가 있습니다:
* Helios 소스를 [Plutus-Core](https://github.com/input-output-hk/plutus)로 컴파일합니다.
* Cardano 블록체인에 트랜잭션을 빌드하고 제출합니다.

## 코드 예제

```helios
// 모든 Helios 프로그램은 스크립트 목적으로 시작합니다.
spending always_true 

// 'main' 함수에는 핵심 검증자 로직이 포함됩니다.
// 주어진 UTxO가 사용될 수 있는지 여부를 반환합니다.
func main() -> Bool {
    // Helios는 표현 기반 언어입니다.
    true
}
```

## 이 책의 구조

Helios를 사용하여 스마트 컨트랙트을 생성하고 DApps를 구축하기 전에, Cardano의 eUTxO 모델을 잘 이해하는 것이 중요합니다. 아직 이해하지 못했다면, 먼저 [eUTxOs 이해하기](./understanding-eutxos.md) 서문을 읽어보시길 권장합니다.

[1장](./lang/index.md)에서는 Helios 내장 기능의 완전한 참조를 포함하여 언어 자체에 대해 다룹니다.

[2장](./api/index.md)에서는 Helios 라이브러리 설정, 스마트 컨트랙트 컴파일, 자바스크립트만 사용하여 스마트 컨트랙트 트랜잭션 빌드 및 제출 방법을 다룹니다.

[3장](./cli/index.md)에서는 *cardano-cli*와 함께 Helios 스마트 컨트랙트 사용 방법을 다룹니다.

[4장](./advanced-concepts/index.md)에서는 발행 정책, 인식해야 할 취약점, 좀 더 복잡한 스크립트 및 DApps 구축을 위한 일부 권장 사항을 다룹니다.
