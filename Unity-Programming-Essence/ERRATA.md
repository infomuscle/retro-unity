# 오탈자와 오류

이 곳은 [**레트로의 유니티 게임 프로그래밍 에센스**](http://www.yes24.com/24/goods/69320872)에서 발견된 오탈자와 수정 내용을 확인할 수 있는 페이지입니다.

## 신고 경로

책의 오탈자와 예제 프로젝트의 잘못된 점은 아래 경로 중 한곳에 신고하면 됩니다.

- [한빛미디어 웹페이지](http://www.hanbit.co.kr/store/books/look.php?p_code=B3604463061) | [깃허브 프로젝트 페이지](https://github.com/IJEMIN/Unity-Programming-Essence) | [저자 유튜브](https://youtube.com/c/JeminDev) | [저자 블로그](https://ijemin.com) | [저자 이메일](i_jemin@outlook.com)

## 오탈자

### P117 마지막줄

- **오타**

> 브로드케이팅으로 Dance()를 가진

- **수정**

> 브로드캐스팅으로 Dance()를 가진

### P193

- **오타**

> punlic name;

- **수정**

> public name;

### P289

- **오타**

> 수정사항이 적용했으니

- **수정**

> 수정사항을 적용했으니

### P294

- **오타**

> Random.Range() 메서드는 입력으로 최댓값과 최솟값을 순서대로

- **수정**

> Random.Range() 메서드는 입력으로 최솟값과 최댓값을 순서대로

### P295

- **오타**

> 누적된 시간을 저장하는 변수 timeSpawnRate를 체크합니다.

- **수정**

> 누적된 시간을 저장하는 변수 timeAfterSpawn를 체크합니다.

### P338

- **오타**

> SampleManager.LoadScene(0);

- **수정**

> SceneManager.LoadScene(0);

### P341

- **오타**

> string 저장/가져오기<br>- **`PlayerPrefs.SetString(string key, float value);`**<br>- `PlayerPrefs.GetString(string key);`

- **수정**

> string 저장/가져오기<br>- **`PlayerPrefs.SetString(string key, string value);`**<br>- `PlayerPrefs.GetString(string key);`

### P407

- **오타**

> 왼쪽 방향키나 아래쪽 방향키

- **수정**

> 왼쪽 방향키나 오른쪽 방향키

### P432

- **오타**

> **오디오 소스 컴포넌트**가 게임속에서 듣는 소리가 게임에 최종출력되는 소리가 됩니다.

> **오디오 컴포넌트**가 오디오 리스너 컴포넌트를 가진 게임 오브젝트에 가까워질수록 해당 **오디오 컴포넌트**의 소리가 크게 들립니다.

- **수정**

> **오디오 리스너 컴포넌트**가 게임속에서 듣는 소리가 게임에 최종출력되는 소리가 됩니다.

> **오디오 소스 컴포넌트**가 오디오 리스너 컴포넌트를 가진 게임 오브젝트에 가까워질수록 해당 **오디오 소스 컴포넌트**의 소리가 크게 들립니다.

### P529, P537

- **오타**

다른 페이지에서는 poolPosition에 (0, -25)가 할당되어 있지만 위 두 페이지에서는 poolPosition에 (0, -20)을 할당합니다.

> `private Vector2 poolPosition = new Vector2(0, -20);`

- **수정**

> `private Vector2 poolPosition = new Vector2(0, -25);`

poolPosition의 값은 화면에 보이지 않을 정도로 원점에서 멀리 떨어진 위치 값이면 어떠한 값이라도 좋습니다.
따라서 (0, -20)과 (0, -25) 중에서 어느쪽을 사용해도 상관없지만, 통일성을 위해 (0, -25)로 통일합니다.

### P530

- **오타**

> **timeSpawn** 위에 선언된 timeBetSpawnMin, timeBetSpawnMax는 timeBetSpawn의 최솟값과 최댓값을 결정합니다.

- **수정**

> **timeBetSpawn** 위에 선언된 timeBetSpawnMin, timeBetSpawnMax는 timeBetSpawn의 최솟값과 최댓값을 결정합니다.

### P532

- **오타**

> poolPosition의 값은 (0, -25)이므로 복제 생성된 발판은 게임 화면에서 **왼쪽**으로 멀리 벗어나 보이지 않습니다.

- **수정**

> poolPosition의 값은 (0, -25)이므로 복제 생성된 발판은 게임 화면에서 **아래쪽**으로 멀리 벗어나 보이지 않습니다.

### P592, 593

- **오타**

예제 코드 상에서는 `Vector3 moveDistance;`를 사용했으나, 본문에서 해당 변수를 **move**라는 이름으로 언급했습니다.

- **수정**

P592, 593에서 언급된 **move** 변수는 **moveDistance** 를 가리키는 것입니다.

### P670

- **오타**

```
void Start() {
    onClean += CleanRoomA;
    onClean += CleanRoomB;
}
```

- **수정**

```
void Start() {
    onClean += CleaningRoomA;
    onClean += CleaningRoomB;
}
```

### P872

- **오타**

> Destroy() 대신 Photon.Network.Destroy() 메서드 사용

- **수정**

> Destroy() 대신 PhotonNetwork.Destroy() 메서드 사용

### P886

- **오타**

> AddScore() 메서드가 실행도록

- **수정**

> AddScore() 메서드가 실행되도록

### P893

- **오타**

> Awake() 메서드에서 Photon.Peer.RegisterType() 실행

- **수정**

> Awake() 메서드에서 PhotonPeer.RegisterType() 실행
