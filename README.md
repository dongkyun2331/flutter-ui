import 'package:flutter/material.dart';

void main() {
  runApp(App());
}

class App extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      home: Scaffold(
        backgroundColor: Color(0xFF181818), // 배경색을 직접 정의한 색상으로 설정
        body: Padding(
          padding: EdgeInsets.symmetric(horizontal: 40), // 가로 방향으로 좌우에 40의 패딩을 추가
          child: Column(
            children: [
              SizedBox(
                height: 80, // 위쪽에 80의 공간을 비움
              ),
              Row(
                mainAxisAlignment: MainAxisAlignment.end, // 가로 정렬을 오른쪽으로 설정
                children: [
                  Column(
                    crossAxisAlignment: CrossAxisAlignment.end, // 세로 정렬을 오른쪽으로 설정
                    children: [
                      Text(
                        'Hey, Selena', // 화면에 표시되는 첫 번째 텍스트
                        style: TextStyle(
                          color: Colors.white, // 텍스트 색상을 흰색으로 설정
                          fontSize: 28, // 폰트 크기 설정
                          fontWeight: FontWeight.w800, // 글꼴 두께를 설정
                        ),
                      ),
                      Text(
                        'Welcome back', // 화면에 표시되는 두 번째 텍스트
                        style: TextStyle(
                          color: Color.fromRGBO(255, 255, 255, 0.8), // 텍스트 색상을 흰색과 투명도 0.8로 설정
                          fontSize: 18, // 폰트 크기 설정
                        ),
                      ),
                    ],
                  )
                ],
              )
            ],
          ),
        ),
      ),
    );
  }
}
