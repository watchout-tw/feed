# Feed Of Wathcout

## Release Notes

### 2018/08/06

- 發佈資料格式版本 v1.0.0
- 新增「各城市下各候選人相關之最熱門提問」資料集

## Datasets

### ask/Candidate Popular Questions

[給問擂台] 各城市下各候選人相關之最熱門提問

### 資料位置

- [台北市](https://feed.watchout.tw/ask/candidate-popular-questions/2018-taipei-candidate-popular-questions.json)
- [新北市](https://feed.watchout.tw/ask/candidate-popular-questions/2018-new-taipei-candidate-popular-questions.json)
- [桃園市](https://feed.watchout.tw/ask/candidate-popular-questions/2018-taoyuan-candidate-popular-questions.json)
- [台中市](https://feed.watchout.tw/ask/candidate-popular-questions/2018-taichung-candidate-popular-questions.json)
- [台南市](https://feed.watchout.tw/ask/candidate-popular-questions/2018-tainan-candidate-popular-questions.json)
- [高雄市](https://feed.watchout.tw/ask/candidate-popular-questions/2018-kaohsiung-candidate-popular-questions.json)

### 資料格式說明

#### 範例

``` json
}
  "formatVersion": "資料格式版本號碼",  // 資料格式版本號碼
  "lastBuildDate": 1533522837782, // 資料最後更新時間
  "uuid": "ask-candidatePopularQuestions-2018-taichung-1533522837782", //資料uuid
  "data": [
    {
      "candidate": { // 參選人資料
        "url": "https://park.watchout.tw/personas/218", //參選人個人頁面
        "name": "林佳龍", //參選人姓名
        "party": { //參選人所屬政黨資訊
          "name": "民主進步黨", //所屬政黨名稱
          "abbreviation": "民進黨", //所屬政黨縮寫
          "color": "#009A00" //所屬政黨代表色
        },
        "questions": [ //參選人相關提問
          {
            "url": "https://ask.watchout.tw/games/2018-taichung/questions/648", //提問網址
            "topic": "性別", //提問議題類別 [註1]
            "title": "兩位對於台中市性別與同志平權議題的想法？會有什麼支持政策？", //提問標題
            "content": "今年年底的公投有婚姻平權公投，也表示同志議題與相關政策，也是政治人物必須面對與表態的議題。台灣的同志大遊行一直都是亞洲重要指標，世界各國也關注台灣的婚姻平權進展。台中這幾年來也曾舉辦多次在地同志遊行。這項議題看似是中央政府的意見，但作為地方政府也有許多可以施力的地方：\n●請問林佳龍：目前台中有哪些進行中的同志友善政策或措施？\n\n●請問盧秀燕：盧秀燕過去不管是在新聞、相關團體中，都未曾對同志議題表態。想請為盧委員理由是？若您上任，會有哪些對於同志友善的政策或措施？\n", //提問內容
            "push": 128, //目前連署數
            "threshold": 100 //連署門檻
          },
  ]
}
```

[註1] : [議題類別清單API](https://core.watchout.tw/park/topics?type=watchout)