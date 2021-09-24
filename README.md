# IPTV 

github를 explore하는 도중 재미있는 url을 발견해서 만들어봤습니다.  
https://github.com/iptv-org/iptv    
 - Collection of publicly available IPTV channels from all over the world 

 <br>

JSON format으로 데이터를 제공해줍니다.  
 전세계에 있는 지역과 채널의 카테고리를 기준으로 채널 이름을 검색할 수 있게 해줍니다.  

 ## Requirements
 - Python 3.6+

 ## Installation

 
```
pip install iptvname==0.0.2
```


 - [나라별 코드 정보](regions.json)
 - [채널별 카테고리 이름 정보](categories.json)

<br> 

 # How to use?

 ```
from iptvname import iptv

korea_channel_data = iptv.channel_by_region('kr')
Animation_channel_data = iptv.channel_by_categories('Animation')

print(korea_channel_data)
print(Animation_channel_data)
 ```

 ```
['Animax Korea', 'AniPlus (Malay subtitles)', 'Arirang', 'Arirang', 'Arirang', 'Arirang', 'Arirang Radio', 'Arirang Radio', 'BBS Buddhist Broadcasting', 'CBS', 'CBS', 'CBS', 'CGNTV', 'Channel 67', 'CJB청주방송 (SBS 淸州)', 'CTS기독교TV', 'EBS 1', 'EBS 1', 'EBS 2', 'EBS e', 'EBS KIDS', 'EBS Kids', 'EBS Plus 1', 'EBS Plus 2', 'EBS+ 1', 'EBS+ 2', 'EBSe', 'Edaily TV', 'GCN', 'Gugbang TV', 'Hallypop', 'JIBS SBS', 'JTBC', 'K+', 'KBC 광주방송 (SBS 光州)', 'KBS 1', 'KBS 1', 'KBS2', 'KBS LiveCam DokDo', 'KBS World', 'KCTV 광주 CH05', 'KTV', 'Maeil Business Newspaper', 'MBC', 'Mnet', 'MTN', 'NBS Korea Agricultural Broadcasting', 'One (Indonesian Sub)', 'SBS', 'SBS International', 'SBS KNN', 'SBS Plus', 'SBS Star', 'TBC 대구 (SBS 大邱)', 'TBS', 'TBS', 'TJB 대전방송 (SBS 大田)', 'TVWorkNet', 'YTN', 'YTN DMB', 'YTN SCIENCE', 'YTN SCIENCE', '가요TV', '국악방송', '대구 MBC (MBC Daegu)', '대전MBC (MBC Daejeon)', '여수MBC (MBC Yeosu)', '제주 MBC (MBC Jeju)', '춘천MBC (MBC Chuncheon)', '한국선거방송']
['Adult Swim Aqua Teen Hunger Force', 'Adult Swim Rick and Morty', 'Adult Swim Robot Chicken', 'Adult Swim Samurai Jack', 'Adult Swim The Venture Bros', 'Animax Japan (English Subs)', 'Animax Japan (Indonesian Subs)', 'Animax Japan (Indonesian Subs)', 'Animax Japan (Thai Subs)', 'Animax Japan (Vietnamese Subs)', 'Animax Japan (Vietnamese Subs)', 'Animax Korea', 'Anime TV', 'Anime Zone TV', 'AT-X', 'CONtv Anime', 'CONtv Anime', 'CONtv Anime', 'CONtv Anime', 'CONtv Anime', 'CONtv Anime', 'CONtv Anime', 'Kanade TV', 'Locomotion TV', 'Locomotion TV', 'Persiana Junior', 'Pluto TV Anime', 'Pluto TV Anime', 'Pluto TV Animé Acción', 'Pluto TV Anime All Ages', 'Pluto TV Anime All Day', 'Pluto TV Anime All Day', 'Pluto TV Anime All Day', 'Pluto TV Anime All Day', 'Pluto TV Animé All Day', 'Pluto TV Animé All Day', 'Pluto TV Anime Clásico', 'Pluto TV Naruto', 'Pluto TV Naruto', 'Pluto TV Naruto', 'Pluto TV Naruto', 'Project Boom']
```