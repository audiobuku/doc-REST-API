__AudioBuku API Reference__

API Base URL

https://api.audiobuku.com

**HTTP(S) Request / HTTP(S) Header**

| Header | Value |
| --- | --- |
| Content-Type | application/json |
| Accept | application/json |
| Authorization | Bearer key |

## List API Methods
| End Point | HTTP Method | Deskripsi |
| --- | --- | --- |
| [`/api/v1/collections`](#collections1) | GET | Show data audiobook filter by collection id |
| [`/api/v1/audiobooks?collection_id={id}`](#audiobooks1) | GET | Show data audiobooks filter by collection id |
| [`/api/v1/audiobooks?category_id={id}`](#audiobooks1) | GET | Show data audiobooks filter by category audiobook id |
| [`/api/v1/audiobooks?narrator_id={id}`](#audiobooks1) | GET | Show data audiobooks filter by narrator id |
| [`/api/v1/audiobooks?author_id={id}`](#audiobooks1) | GET | Show data audiobooks filter by author id |
| [`/api/v1/audiobooks?publisher_book_id={id}`](#audiobooks1) | GET | Show data audiobooks filter by publisher book id |
| [`/api/v1/audiobooks?publisher_audiobook_id={id}`](#audiobooks1) | GET | Show data audiobooks filter by publisher audio id |
| [`/api/v1/audiobooks?search={character}`](#audiobooks1) | GET | Show data audiobook filter by character or title book, narrator, publisher book, author |
| [`/api/v1/audiobooks/{id}`](#audiobook) | GET | Show all data audiobook filter by id audiobook |
| [`/api/v1/categories`](#category) | GET | Show data category audiobook |
| [`/api/v1/categories/{id}`](#category) | GET | Show data subcategory audiobook |

<a name="collections1"/>
## Result collection  

```json
[
    {
        "id": 338,
        "title": "Best Seller",
        "picture_url": null,
        "subtitle": "most wanted audiobook",
        "visibility": 1,
        "audiobook": [
            {
                "id": 631,
                "cover_picture_url": "https://storage.googleapis.com/audiobukucover/631_20170202061506.png",
                "title": "Keluarga Tak Kasat Mata",
                "pivot": {
                    "collection_id": 338,
                    "audiobook_id": 631
                }
            }
        ]
    }
]
```


<a name="audiobooks1"/>
## Result audiobooks  

```json
[
    {
        "id": 631,
        "title": "Keluarga Tak Kasat Mata",
        "cover_picture_url": "https://storage.googleapis.com/audiobukucover/631_20170202061506.png",
        "updated_at": "2019-07-05 08:33:50",
        "price": 75000,
        "author": "Bonaventura Genta",
        "created_at": "2017-02-02 12:45:35",
        "released_at": "2019-06-14 13:02:46",
        "audiobook_id": 631,
        "reviews_count": 10,
        "ratings_average": 4.1,
        "wishlisted": null,
        "purchased": null,
        "review": [
            {
                "id": 5745,
                "rating": 3,
                "content": "lumayan lahh . first horror story gue nih",
                "created_at": "2017-12-29 12:50:45",
                "updated_at": "2017-12-29 12:50:45",
                "name": "riezka rahma",
                "photo_url": "https://lh3.googleusercontent.com/-0F1d6t5LSLI/AAAAAAAAAAI/AAAAAAAAAHo/qEtJE25RCYc/s96-c/photo.jpg"
            }
        ],
        "purchase_count": 209,
        "authorslist": [
            {
                "audiobook_id": 631,
                "id": 53,
                "username": "Bonaventura Genta",
                "photo_url": null
            }
        ],
        "narratorslist": [
            {
                "audiobook_id": 631,
                "id": 37,
                "username": "Dian Tedjo",
                "photo_url": null
            }
        ]
    }
    ]
```



<a name="audiobook"/>
## Result audiobook  

```json
{
    "id": 631,
    "title": "Keluarga Tak Kasat Mata",
    "subtitle": "Gagas Media",
    "author": "Bonaventura Genta",
    "narrator": "Dian Tedjo, dkk",
    "isbn": "9786021472868",
    "price": 75000,
    "about": "Saya berbalik arah, tapi di belakang sudah menanti sosok si Nenek Bermukena yang sepertinya sudah mengamati saya sedari tadi. “Ngopo koe ning kene? Balik saiki!” (Kenapa kamu di sini? Pulang sekarang!) \r\n\r\nDapatkan Print Buku nya! Kunjungi Web : <a href=\"http://gagasmedia.net/component/virtuemart/kumpulan-cerita-prosa/keluarga-tak-kasatmata-detail?Itemid=483\">Penerbit Gagas Media</a>",
    "audio_preview_file_url": "https://storage.googleapis.com/audiobukupreview/631_20170202054535.mp3",
    "cover_picture_url": "https://storage.googleapis.com/audiobukucover/631_20170202061506.png",
    "duration_seconds": 12522,
    "duration_second_preview": 180,
    "copyright_year": "2017",
    "visibility": 0,
    "released_at": "2019-06-14 13:02:46",
    "approve": 1,
    "mature_content": 0,
    "created_at": "2017-02-02 12:45:35",
    "updated_at": "2019-07-05 14:26:00",
    "deleted_at": null,
    "published": null,
    "category_id": 112,
    "publisher_audiobook_id": 2,
    "publisher_book_id": 28,
    "type_audiobook_id": 1,
    "viewer": 227,
    "similar": [
        {
            "best_seller": 209,
            "id": 631,
            "cover_picture_url": "https://storage.googleapis.com/audiobukucover/631_20170202061506.png",
            "mature_content": 0
        },
        {
            "best_seller": 114,
            "id": 1473,
            "cover_picture_url": "https://storage.googleapis.com/audiobukucover/1473_20171208033739.png",
            "mature_content": 0
        },
        {
            "best_seller": 86,
            "id": 1041,
            "cover_picture_url": "https://storage.googleapis.com/audiobukucover/1041_20171002020426.png",
            "mature_content": 0
        },
        {
            "best_seller": 32,
            "id": 1091,
            "cover_picture_url": "https://storage.googleapis.com/audiobukucover/1091_20171017180744.png",
            "mature_content": 0
        },
        {
            "best_seller": 27,
            "id": 1092,
            "cover_picture_url": "https://storage.googleapis.com/audiobukucover/1092_20171017190820.png",
            "mature_content": 0
        },
        {
            "best_seller": 8,
            "id": 1471,
            "cover_picture_url": "https://storage.googleapis.com/audiobukucover/1471_20171205033720.png",
            "mature_content": 1
        },
        {
            "best_seller": 1,
            "id": 3049,
            "cover_picture_url": "https://storage.googleapis.com/audiobukucover/4fb37fad-d025-49be-9fd9-b6a3f97ec54c.png",
            "mature_content": 0
        }
    ],
    "reviews_count": 10,
    "ratings_average": 4.1,
    "wishlisted": null,
    "purchased": null,
    "review": [
        {
            "id": 5745,
            "rating": 3,
            "content": "lumayan lahh . first horror story gue nih",
            "created_at": "2017-12-29 12:50:45",
            "updated_at": "2017-12-29 12:50:45",
            "name": "riezka rahma",
            "photo_url": "https://lh3.googleusercontent.com/-0F1d6t5LSLI/AAAAAAAAAAI/AAAAAAAAAHo/qEtJE25RCYc/s96-c/photo.jpg"
        },
        {
            "id": 5743,
            "rating": 3,
            "content": "kok ngak bisa beli,, provaider indosat",
            "created_at": "2017-12-22 00:22:48",
            "updated_at": "2017-12-22 00:22:48",
            "name": "Bagus Rumaji",
            "photo_url": null
        },
        {
            "id": 5742,
            "rating": 5,
            "content": "naratornya top",
            "created_at": "2017-12-20 15:43:10",
            "updated_at": "2017-12-20 15:43:10",
            "name": "",
            "photo_url": null
        },
        {
            "id": 5741,
            "rating": 0,
            "content": "Cara bayarnya gimana? Pake pulsa boleh nggak? ",
            "created_at": "2017-12-20 15:24:50",
            "updated_at": "2017-12-20 15:24:50",
            "name": "naufa izzul ummam",
            "photo_url": "https://lh6.googleusercontent.com/-g9bl9YNZqNA/AAAAAAAAAAI/AAAAAAAAAJ0/IZ8PbJv0CZk/s96-c/photo.jpg"
        },
        {
            "id": 5718,
            "rating": 5,
            "content": "saran aja untuk bagian2 yg berbahasa jawa tlg disediakan artinya. sy tdk mengerti artinya. \n",
            "created_at": "2017-11-03 19:20:42",
            "updated_at": "2017-11-03 19:20:42",
            "name": "Metri Pradnyani",
            "photo_url": "https://lh3.googleusercontent.com/-H7BnYfQliDQ/AAAAAAAAAAI/AAAAAAAAAAA/AAnnY7o9q_JPi4qp47aSyE-xhchHCcUzPg/s96-c/photo.jpg"
        }
    ],
    "purchase_count": 209,
    "authorslist": [
        {
            "audiobook_id": 631,
            "id": 53,
            "username": "Bonaventura Genta",
            "photo_url": null
        }
    ],
    "narratorslist": [
        {
            "audiobook_id": 631,
            "id": 37,
            "username": "Dian Tedjo",
            "photo_url": null
        }
    ],
    "publisherbook": {
        "name": "Gagas Media",
        "id": 28,
        "photo_url": "https://storage.googleapis.com/audiobukucover/8d522767-a104-4fb7-8c25-e0812e79f6de.jpg"
    },
    "publisheraudiobook": {
        "name": "PT. Edifikasi Media Indonesia (AudioBuku)",
        "id": 2,
        "photo_url": "https://storage.googleapis.com/audiobukucover/a0126fa5-41be-4e1f-825e-e22119b3e431.jpg"
    },
    "audiobookchapter": [
        {
            "id": 3914,
            "title": "KTKM01 - Bagian 1",
            "subtitle": "Gagas Media",
            "price": 15000,
            "about": "KTKM01 - Bagian 1",
            "cover_picture_url": "https://storage.googleapis.com/audiobukucover/3914_20170202061534.png",
            "duration_seconds": 1999,
            "sequence": 0,
            "created_at": "2017-02-02 12:46:36",
            "updated_at": "2019-03-11 13:59:08",
            "deleted_at": null,
            "audiobook_id": 631
        },
        {
            "id": 3915,
            "title": "KTKM01 - Bagian 2",
            "subtitle": "Gagas Media",
            "price": 15000,
            "about": "KTKM01 - Bagian 2",
            "cover_picture_url": "https://storage.googleapis.com/audiobukucover/3915_20170202061552.png",
            "duration_seconds": 1516,
            "sequence": 0,
            "created_at": "2017-02-02 12:47:38",
            "updated_at": "2019-03-11 13:59:28",
            "deleted_at": null,
            "audiobook_id": 631
        },
        {
            "id": 3930,
            "title": "KTKM02 - Bagian 1",
            "subtitle": "Gagas Media",
            "price": 12500,
            "about": "KTKM02 - Bagian 1",
            "cover_picture_url": "https://storage.googleapis.com/audiobukucover/3930_20170203082240.png",
            "duration_seconds": 1459,
            "sequence": 0,
            "created_at": "2017-02-03 14:16:08",
            "updated_at": "2019-03-11 14:01:19",
            "deleted_at": null,
            "audiobook_id": 631
        },
        {
            "id": 3931,
            "title": "KTKM02 - Bagian 2",
            "subtitle": "Gagas Media",
            "price": 15000,
            "about": "KTKM02 - Bagian 2",
            "cover_picture_url": "https://storage.googleapis.com/audiobukucover/3931_20170203082221.png",
            "duration_seconds": 1707,
            "sequence": 0,
            "created_at": "2017-02-03 14:16:58",
            "updated_at": "2019-03-11 14:00:55",
            "deleted_at": null,
            "audiobook_id": 631
        },
        {
            "id": 3932,
            "title": "KTKM03 - Bagian 1",
            "subtitle": "Gagas Media",
            "price": 15000,
            "about": "KTKM03 - Bagian 1",
            "cover_picture_url": "https://storage.googleapis.com/audiobukucover/3932_20170203082153.png",
            "duration_seconds": 2369,
            "sequence": 0,
            "created_at": "2017-02-03 14:21:02",
            "updated_at": "2019-03-11 14:02:23",
            "deleted_at": null,
            "audiobook_id": 631
        },
        {
            "id": 3933,
            "title": "KTKM03 - Bagian 2",
            "subtitle": "Gagas Media",
            "price": 15000,
            "about": "KTKM03 - Bagian 2",
            "cover_picture_url": "https://storage.googleapis.com/audiobukucover/3933_20170203082128.png",
            "duration_seconds": 1651,
            "sequence": 0,
            "created_at": "2017-02-03 14:21:38",
            "updated_at": "2019-03-11 14:02:49",
            "deleted_at": null,
            "audiobook_id": 631
        },
        {
            "id": 3935,
            "title": "KTKM04 - Penutup",
            "subtitle": "Gagas Media",
            "price": 15000,
            "about": "KTKM04 - Penutup",
            "cover_picture_url": "https://storage.googleapis.com/audiobukucover/3935_20170203082055.png",
            "duration_seconds": 1821,
            "sequence": 0,
            "created_at": "2017-02-03 15:13:40",
            "updated_at": "2019-03-11 14:03:42",
            "deleted_at": null,
            "audiobook_id": 631
        }
    ],
    "category": {
        "id": 112,
        "title": "HOROR & MISTERI",
        "parent": null
    }
}
```

<a name="category"/>
## Result category  

```json
{
    "error": true,
    "userMessage": "success",
    "data": [
        {
            "id": 83,
            "title": "BELAJAR BAHASA",
            "picture_url": "https://storage.googleapis.com/audiobukucover/456_20161227175855.jpg"
        },
        {
            "id": 99,
            "title": "BIOGRAFI & MEMOAR",
            "picture_url": "https://storage.googleapis.com/audiobukucover/490_20161226030219.jpg"
        }
    ]
}
```
