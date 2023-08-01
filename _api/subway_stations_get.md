---
title: /urban/api/subway_geojson.php
position_number: 3.1
type: get
description: Get subway coordinates
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
        {"type" : "FeatureCollection", "features" : [{"type": "Feature", "geometry": {"type":"Point","coordinates":[126.975271,37.563534]}, "properties": {"철도운영기관명": "서울교통공사", "노선": "2호선", "역명": "시청", "경도": 126.975271, "위도": 37.563534}}, ...]}
      }
    title: Response
    language: json
---
