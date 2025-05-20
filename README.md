*2018 Nov. new!* [thinkingo at PAMS 2018](https://github.com/HongBeenKim/pams-skku)

# HEVEN Autonomous Car 2018 (English Translated)

2018 International Student Car Competition: Autonomous Car SKKU Team. HEVEN

2018 International Student Creative Car Competition, Autonomous Driving Division, Sungkyunkwan University Team HEVEN

\[Awarded Encouragement Prize] [Final round live stream recording (from 1:25:20)](https://tv.naver.com/v/3246704)
`The live stream recording contains original stream interruptions, so the video may have brief freezes.`

[Post-competition review article](https://jueun-park.github.io/2018-07-08/postscript-autonomous-car)

[Official Website of the International Student Car Competition](http://kasa.kr/cev/)

---

## Autonomous Driving Program Structure

`./src/program_name.py`

### Program Roles

| Category          | Role                                  | Program Name                             |                       Developer                       |
| :---------------- | :------------------------------------ | :--------------------------------------- | :---------------------------------------------------: |
| **Perception**    | LiDAR Mapper                          | `lidar.py`                               |                      Hongbin Kim                      |
| "                 | Cam Video Stream Control              | `video_stream.py`                        |                      Jinwoong Kim                     |
| "                 | Lane Detector                         | `lane_cam.py`                            |                 Hongbin Kim, Hajin Ye                 |
| "                 | Sign Detector                         | `shape_detection.py`<br>`sign_cam.py`    | Yoonjin Kim, Ahyoung Lee<br>Sungwoo Kim, Jiwoong Hyun |
| **Planning**      | Motion & Particular Condition Planner | `parabola.py`<br>`motion_planner.py`     |                      Hongbin Kim                      |
| **Control**       | Car Speed/Steering Control            | `car_control.py`                         |                      Junhyuk Park                     |
| **Communication** | Communication with Platform           | `serial_packet.py`<br>`communication.py` |                      Jinwoong Kim                     |
| **Process**       | Main Process Management               | `main.py`                                |              Jinwoong Kim, Seongryong Yoo             |

* Project Design & Management: Jueun Park

### Hierarchical Structure

```
main.py
├ communication.py
│ └ serial_packet.py
│ 
├ motion_planner.py
│ ├ lidar.py
│ │ 
│ ├ lane_cam.py
│ │ └ video_stream.py
│ │
│ ├ parabola.py
│ │ 
│ ├ video_stream.py
│ │
│ ├ sign_cam.py
│ │ └ shape_detection.py
│ │
│ └ key_cam.py
│ 
├ car_control.py
│ 
└ monitor.py
```

For detailed descriptions of the development process, refer to the team-authored wiki: [HEVEN\_AutonomousCar\_2018 wiki](https://github.com/Jueun-Park/HEVEN_AutonomousCar_2018/wiki)

---

## Team Members (2018)

### Software & Algorithm Development Division (10)

* Sungwoo Kim: Industrial Management Engineering / Computer Engineering
* Yoonjin Kim: Department of Electrical and Electronic Engineering
* Jinwoong Kim: Computer Engineering
* Hongbin Kim: Department of Mechanical Engineering
* Jueun Park: Industrial Management Engineering / Informatics
* Junhyuk Park: Department of Electrical and Electronic Engineering
* Hajin Ye: School of Engineering
* Seongryong Yoo: Department of Electrical and Electronic Engineering
* Ahyoung Lee: Department of Materials Science & Engineering / Department of Electrical and Electronic Engineering
* Jiwoong Hyun: School of Software

### Vehicle Exterior Division (3)

* Heesoo Kang: Department of Sports Science / Department of Mechanical Engineering
* Minsu Kim: Department of Mechanical Engineering
* Joonggu Lee: Department of Mechanical Engineering / Department of Electrical and Electronic Engineering

![Team. HEVEN\_A Group Photo](https://github.com/Jueun-Park/HEVEN_AutonomousCar_2018/blob/master/img_for_md/\(%EC%A0%80%ED%99%94%EC%A7%88\)2018%ED%97%A4%EB%B8%90%EC%9E%90%EC%9C%A8%EC%B0%A8%ED%8C%80%EB%8B%A8%EC%B2%B4%EC%82%AC%EC%A7%84.jpg)

\[Photo. 2018 Team. HEVEN\_Autonomous\_Car Members [(original photo)](https://github.com/Jueun-Park/HEVEN_AutonomousCar_2018/blob/master/img_for_md/%28%EC%88%98%EC%A0%95%292018%ED%97%A4%EB%B8%90%EC%9E%90%EC%9C%A8%EC%B0%A8%ED%8C%80%EB%8B%A8%EC%B2%B4%EC%82%AC%EC%A7%84.jpg)]
`Note: One member is missing in the above photo due to circumstances.`

---

## Competition Results

![Final Results - Autonomous Division](https://github.com/Jueun-Park/HEVEN_AutonomousCar_2018/blob/master/img_for_md/2018%EB%85%84%EA%B5%AD%EC%A0%9C%EB%8C%80%ED%95%99%EC%83%9D%EC%B0%BD%EC%9E%91%EC%9E%90%EB%8F%99%EC%B0%A8%EA%B2%BD%EC%A7%84%EB%8C%80%ED%9A%8C-%EC%9E%90%EC%9C%A8%EC%B0%A8%EB%B6%80%EB%AC%B8%EC%B5%9C%EC%A2%85%EA%B2%B0%EA%B3%BC.JPG)

\[Table. Final Results - 2018 International Student Creative Car Competition - Autonomous Division]

![Final Round Driving Results - Autonomous Division](https://github.com/Jueun-Park/HEVEN_AutonomousCar_2018/blob/master/img_for_md/2018%EB%85%84%EA%B5%AD%EC%A0%9C%EB%8C%80%ED%95%99%EC%83%9D%EC%B0%BD%EC%9E%91%EC%9E%90%EB%8F%99%EC%B0%A8%EA%B2%BD%EC%A7%84%EB%8C%80%ED%9A%8C-%EC%9E%90%EC%9C%A8%EC%B0%A8%EB%B6%80%EB%AC%B8%EB%B3%B8%EC%84%A0%EC%A3%BC%ED%96%89%EA%B2%B0%EA%B3%BC.JPG)

\[Table. Final Round Driving Results - 2018 International Student Creative Car Competition - Autonomous Division]

![Preliminary Round Driving Results - Autonomous Division](https://github.com/Jueun-Park/HEVEN_AutonomousCar_2018/blob/master/img_for_md/2018%EB%85%84%EA%B5%AD%EC%A0%9C%EB%8C%80%ED%95%99%EC%83%9D%EC%B0%BD%EC%9E%91%EC%9E%90%EB%8F%99%EC%B0%A8%EA%B2%BD%EC%A7%84%EB%8C%80%ED%9A%8C-%EC%9E%90%EC%9C%A8%EC%B0%A8%EB%B6%80%EB%AC%B8%EC%98%88%EC%84%A0%EC%A3%BC%ED%96%89%EA%B2%B0%EA%B3%BC.JPG)

\[Table. Preliminary Round Driving Results - 2018 International Student Creative Car Competition - Autonomous Division]

---

![Awards Summary](https://github.com/Jueun-Park/HEVEN_AutonomousCar_2018/blob/master/img_for_md/2018%EB%85%84%EA%B5%AD%EC%A0%9C%EB%8C%80%ED%95%99%EC%83%9D%EC%B0%BD%EC%9E%91%EC%9E%90%EB%8F%99%EC%B0%A8%EA%B2%BD%EC%A7%84%EB%8C%80%ED%9A%8C%EA%B2%B0%EA%B3%BC.jpg)

\[Table. Award Summary - 2018 International Student Creative Car Competition]

---

## Credit

[HEVEN\_AutonomousCar\_2017](https://github.com/jungAcat/HEVEN_AutonomousCar_2017) (2017 International Student Creative Car Competition, Autonomous Division, Sungkyunkwan University Team HEVEN)
