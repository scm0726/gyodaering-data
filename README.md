# gyodaering-data

교대링 앱의 **회사 근무표 목록**이에요.

- 앱은 `companies.json`을 읽어서 '회사 근무표 찾기'에 보여줘요.
- 이 파일은 관리자 페이지(gyodaering-admin.html)에서 근무표를 승인하고 'GitHub에 저장'을 누르면 자동으로 바뀌어요. 직접 고칠 일은 거의 없어요.
- 앱이 로그인 없이 읽어야 해서 저장소는 **공개(Public)**로 유지해야 해요.

## companies.json 형식

```json
{
  "v": 1,
  "updated": "2026-11-19",
  "companies": [
    {
      "key": "한빛화학-울산공장",
      "name": "한빛화학",
      "region": "울산공장",
      "dept": "생산",
      "note": "",
      "ver": 1,
      "added": "2026-11-19",
      "updated": "2026-11-19",
      "c": {
        "baseDate": "2026-01-05",
        "types": [{ "id": "d1", "name": "1직", "label": "1", "color": "#FFCF1A" }],
        "pattern": ["d1", "d1", "off"],
        "teams": [{ "id": "t1", "name": "1조", "offset": 0 }]
      }
    }
  ]
}
```

회사가 근무표 공개를 원하지 않으면 관리자 페이지에서 삭제해 주세요.
