## 공통

### 1) 서버에서 던지는 Response Code

- 200
- 404
- 413
- 500

## 사진 + 식재료 등록 (1)

### 1) 안드로이드 → 스프링 백엔드 사진 분석 요청

요청 URL: POST /analysis/request

이미지 바이너리

응답 결과:

```jsx
{
  "names": [
    {
      "name": "a",
      "bestBefore": unixTimestamp(Long) //안올수도 있음
    },
    {
      "name": "a",
      "bestBefore": unixTimestamp(Long)
    },
    {
      "name": "a",
      "bestBefore": unixTimestamp(Long)
    }
  ]
}
```

## 2) 스프링 → 플라스크 사진 분석 요청

요청 URL: POST /analysis/request

이미지 바이너리

응답 결과:

```jsx
{
  "names": [
    {
      "name": "a"
    },
    {
      "name": "a"
		},
    {
      "name": "a"
		}
  ]
}
```

## 3) 안드로이드 → 스프링 식품 등록

요청 URL: POST /item/add

요청 JSON:

```jsx
{
  "names": [
    {
      "name": "a",
      "bestBefore": unixTimestamp(Long)
    },
    {
      "name": "a",
      "bestBefore": unixTimestamp(Long)
    },
    {
      "name": "a",
      "bestBefore": unixTimestamp(Long)
    }
  ]
}
```

응답: 없음 (200 코드)
