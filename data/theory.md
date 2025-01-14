## data/theory

| arguments      | description                                                                     | optional |
|:---------------|:--------------------------------------------------------------------------------|----------|
| overflow       | number, range 0-10. The number of the overflow records below the best30 minimum | true     |
| with_recent    | boolean. if true, will reply with recent_score                                  | true     |
| with_song_info | boolean. if true, will reply with song_info                                     | true     |
| version        | string, formatted like '4.0'.     The version of Arcaea.                        | true     |

###### Tag

* Enable Cors

#### Example

+ `{apiurl}/arcapi/data/theory?with_recent=true&with_song_info=true&version=3.0`

##### Return data (Edited for readability)

```json5
{
  "status": 0,
  "content": {
    "best30_avg": 12.480000000000002,
    "recent10_avg": 12.870000000000001,
    "account_info": {
      "code": "000000000",
      "name": "Max Grades - v3.0",
      "user_id": 0,
      "is_mutual": false,
      "is_char_uncapped_override": true,
      "is_char_uncapped": true,
      "is_skill_sealed": false,
      "rating": 1257,
      "character": 5
    },
    "best30_list": [
      {
        "score": 10001279,
        "health": 100,
        "rating": 13.3,
        "song_id": "fractureray",
        "modifier": 0,
        "difficulty": 2,
        "clear_type": 3,
        "best_clear_type": 3,
        "time_played": 1531699208,
        "near_count": 0,
        "miss_count": 0,
        "perfect_count": 1279,
        "shiny_perfect_count": 1279
      }
    ],
    "best30_song_info": [
      {
        "name_en": "Fracture Ray",
        "name_jp": "",
        "artist": "Sakuzyo",
        "bpm": "200",
        "bpm_base": 200.0,
        "set": "rei",
        "set_friendly": "Luminous Sky",
        "time": 154,
        "side": 0,
        "world_unlock": false,
        "remote_download": true,
        "bg": "fractureray",
        "date": 1531699208,
        "version": "1.7",
        "difficulty": 22,
        "rating": 113,
        "note": 1279,
        "chart_designer": "Paradox Zero",
        "jacket_designer": "シエラ",
        "jacket_override": false,
        "audio_override": false
      }
    ],
    "recent_score": {
      "score": 10001279,
      "rating": 13.3,
      "song_id": "fractureray",
      "difficulty": 2,
      "time_played": 1531699208
    },
    "recent_song_info": {
      "name_en": "Fracture Ray",
      "name_jp": "",
      "artist": "Sakuzyo",
      "bpm": "200",
      "bpm_base": 200.0,
      "set": "rei",
      "set_friendly": "Luminous Sky",
      "time": 154,
      "side": 0,
      "world_unlock": false,
      "remote_download": true,
      "bg": "fractureray",
      "date": 1531699208,
      "version": "1.7",
      "difficulty": 22,
      "rating": 113,
      "note": 1279,
      "chart_designer": "Paradox Zero",
      "jacket_designer": "シエラ",
      "jacket_override": false,
      "audio_override": false
    }
  }
}
```
