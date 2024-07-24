LINE

### ストア関連
#### 検索
```
https://store.line.me/api/search/{種類}?query={検索}&offset={ページ数}&limit={1ページあたりの量}&type={種類}&includeFacets={includeFacets}
```
- 種類: sticker,emoji,theme,family
- 検索: 検索ワード
- ページ数: 0から始まる
- 1ページあたりの量: nunber
- 種類: SUBSCRIPTION,CREATORS,OFFICIAL,ALLから選択できます。
- includeFacets: booleanで表して最後の行の有無を表す。詳細は下記のレスポンスを参照  
**レスポンス**
```jsonc
{
    "totalCount":"総数",
    "item":[
        {
        "id": "23724",
        "title": "東方LostWord",
        "description": null,
        "newFlag": false,
        "productUrl": "/stickershop/product/23724/ja",
        "listIcon": {
            "src": "https://stickershop.line-scdn.net/stickershop/v1/product/23724/LINEStorePC/main.png?v=1",
            "width": null,
            "height": null,
            "imageId": null
        },
        "type": "STICKER",
        "subtype": "GENERAL",
        "authorId": "2276477",
        "authorName": "GOOD SMILE COMPANY",
        "priceTier": 2,
        "priceAmount": "250",
        "priceString": "￥250",
        "version": 1,
        "versionString": null,
        "validDays": -1,
        "onSale": true,
        "availableForPurchase": true,
        "availableForPresent": true,
        "bargainFlag": false,
        "promotionType": "NONE",
        "stickerResourceType": "STATIC",
        "sticonResourceType": null,
        "hasAnimation": false,
        "hasSound": false,
        "payloadForProduct": {
            "payloadType": "PRODUCT",
            "productId": "23724",
            "stickerId": null,
            "resourceType": "STATIC",
            "staticUrl": "https://stickershop.line-scdn.net/stickershop/v1/product/23724/LINEStorePC/main.png?v=1",
            "fixedStaticUrl": null,
            "animationUrl": null,
            "popupUrl": null,
            "soundUrl": null,
            "collectionStatus": "OFF",
            "addedToCollection": false
        },
        "payloadsToPreviews": [],
        "sticonPayloadForProduct": null,
        "sticonPayloadsToPreviews": [],
        "subscriptionProduct": false,
        "subscriptionOnlyProduct": false,
        "general": true,
        "price": "￥250",
        "creators": false,
        "effectSticker": false
        },
    ],
    "facets":[
        {
        "type": "[SUBSCRIPTION,CREATORS,OFFICIAL,ALL]のいずれか",
        "count": "個数(数値)",
        "overMax": "不明(真偽値)"
        },
    ]
}
```