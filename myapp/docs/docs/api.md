# API 仕様
## POST /api/schedules
説明：ユーザーが入力した授業・バイト・予定を受け取り、データベースに保存する
リクエスト：{"title":"アルバイト",
            "date":"2026-05-12",
            "startTime":"17:00",
            "endTime":"21:00",
            "priority":"high"}
レスポンス：{"message":"予定を登録しました",
            "schedule":{
                "id":1,
                "title":"アルバイト",
                "date":"2026-05-12",
                "startTime":"17:00",
                "endTime":"21:00",
                "priority":"high"
                }
            }

## GET /api/schedules
説明：ログインしているユーザーの予定一覧をデータベースから取得して返す
レスポンス：[{"id":1,
            "title":"アルバイト",
            "date":"2026-05-12",
            "atartTime":"17:00",
            }]