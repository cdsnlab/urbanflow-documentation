---
title: /urban/api/subway_geojson.php
position_number: 3.1
type: get
description: Get Book
parameters:
  - name:
    content:
content_markdown: |-
  Returns a specific book from your collection
left_code_blocks:
  - code_block: |-
      $.get("https://deepurban.kaist.ac.kr/urban/api/subway_geojson.php", {}, function(data) {
        alert(data);
      });
    title: jQuery
    language: javascript
right_code_blocks:
  - code_block: |2-
      {
        "id": 3,
        "title": "The Book Thief",
        "score": 4.3,
        "dateAdded": "5/1/2015"
      }
    title: Response
    language: json
  - code_block: |2-
      {
        {"type" : "FeatureCollection", "features" : [{"type": "Feature", "geometry": {"type":"Point","coordinates":[126.975271,37.563534]}, "properties": {"철도운영기관명": "서울교통공사", "노선": "2호선", "역명": "시청", "경도": 126.975271, "위도": 37.563534}}, ...]}
      }
    title: Error
    language: geojson
---
