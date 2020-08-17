# AI Speaker for Senior Citizen - Test Code

## Solution
### 솔루션 제공 알고리즘

~~~
double today_t ;         #오늘의 온도
double today_h ;         #오늘의 습도
double find_dust ;       #미세먼지 수치
double t ;               #현재 온도
double h;                #현재 습도
if season == 여름 
    if today_t - t = 8 
        print(현재 밖과의 온도차가 매우 큽니다. )
        온도를 높이는 솔루션 제공(에어컨, 선풍기 전원 off)
    
    else
      if t = 30 AND h = 65          온도가 높고 습도도 높은 상태
          print(현재 온도는 높고 습도도 높습니다.)
          
          if find_dust = 나쁨 수치 OR today_h  h  
              온도를 낮추는 솔루션과 습도를 낮추는 솔루션 제공 ( '환기하기' 옵션은 제외)
          else
              온도를 낮추는 솔루션과 습도를 낮추는 솔루션 제공 ( '난방틀기' 제외)
      elif t = 30 AND h = 35      온도가 높고 습도는 낮은 상태
          print(현재 온도는 높고 습도는 낮습니다.)    
          온도를 낮추는 솔루션과 습도를 높이는 솔루션 제공
      elif t = 30 AND  35 h  65    온도만 높은 상태
          print(현재 온도가 높습니다.)
          온도를 낮추는 솔루션 제공
      elif t  30 AND h = 65   습도만 높은 상태
          print(현재 습도가 높습니다.)
          if( find_dust = 나쁨 수치 OR today_h  h)
                  습도를 낮추는 솔루션 제공 (환기시키기 제외)
          else
                  습도를 낮추는 솔루션 제공
      elif t  30 AND h = 35   습도만 낮은 상태
          print(현재 습도가 낮습니다.)
          습도를 높이는 솔루션 제공
      else
          print(현재 온도와 습도가 모두 쾌적한 상태입니다.)
elif season == 겨울 
    if t = 22 AND h = 65 
        print(현재 온도는 낮고 습도도 높습니다.)
        if fine_dust = 나쁨수치 OR today_h = h 
            온도를 높이는 솔루션과 습도를 낮추는 솔루션 제공 (환기 솔루션 제외)
        else
            온도를 높이는 솔루션과 습도를 낮추는 솔루션 제공 (난방 솔루션과 따뜻한 물을 마시는 것이 최적해)
    elif t = 22 AND h = 35 
        print(현재 온도는 낮고 습도는 낮습니다.)
        온도를 높이는 솔루션과 습도를 높이는 솔루션 제공
    elif t = 22 AND 35 h 65 
        print(현재 온도가 낮습니다.)
        온도를 높이는 솔루션 제공
    elif t  22 AND h = 65 
        print(현재 습도가 높습니다.)
        if fine_dust = 나쁨수치 OR today_h = h
            습도를 낮추는 솔루션 제공(환기 솔루션 제외)
        else
            습도를 낮추는 솔루션 제공
    elif t  22 AND h = 35 
        print(현재 습도가 낮습니다.)
        습도를 높이는 솔루션 제공
    else
        print(현재 온도와 습도가 모두 쾌적한 상태입니다.)
else
    if today_t - t = 8 
        print(현재 밖과의 온도 차이가 매우 큽니다.)
        에어컨을 끄거나, 선풍기를 끄도록 유도
    else 
      if 29 = t AND h = 65 
          print(현재 온도가 높고 습도도 높습니다. )
        if fine_dust = 나쁨 수치 OR today_h = h 
              온도를 낮추는 솔루션과  습도를 낮추는 솔루션 제공 (환기 솔루션 제외)
        else
            온도를 낮추는 솔루션과 습도를 낮추는 솔루션 제공
      elif 29 = t AND h = 35 
        print(현재 온도가 높고 습도는 낮습니다. )
        온도를 낮추는 솔루션과 습도를 높이는 솔루션 제공
      elif 22 = t AND h = 65 
          print(현재 온도가 낮고 습도는 높습니다. )
        if fine_dust = 나쁨 수치 OR today_h = h 
            온도를 높이는 솔루션과 습도를 낮추는 솔루션 제공 (환기 솔루션 제외)
        else
            온도를 높이는 솔루션과 습도를 낮추는 솔루션 제공
      elif 22 = t AND h = 35 
        print(현재 온도가 낮고 습도는 낮습니다. )
        온도를 높이는 솔루션과 습도를 높이는 솔루션 제공
      elif 29 = t AND 35  h  65 
        print(현재 온도가 높습니다. )
        온도를 낮추는 솔루션 제공
      elif 22 = t AND 35  h  65
        print(현재 온도가 낮습니다. )
        온도를 높이는 솔루션 제공
      elif 22  t  29 AND h = 65 
        print(현재 습도가 높습니다. )
        if fine_dust = 나쁨 수치 OR today_h = h 
            습도를 낮추는 솔루션 제공 (환기 솔루션 제외)
        else
            습도를 낮추는 솔루션 제공
      elif 22  t  29 AND h = 35 
        print(현재 습도가 낮습니다. )
        습도를 올리는 솔루션 제공
      else
        print(현재 온도와 습도가 모두 쾌적한 상태 입니다.)
~~~
