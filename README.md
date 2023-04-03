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
      "bestBefore": "DateTime.ToString()" //안올수도 있음
    },
    {
      "name": "a",
      "bestBefore": "DateTime.ToString()"
    },
    {
      "name": "a",
      "bestBefore": "DateTime.ToString()"
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
