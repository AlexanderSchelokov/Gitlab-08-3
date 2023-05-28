Задание 1
![image](https://github.com/AlexanderSchelokov/Gitlab-08-3/assets/121572590/a6c593b3-0ef6-4c7d-887b-3a4b153f6118)
![image](https://github.com/AlexanderSchelokov/Gitlab-08-3/assets/121572590/f0ad766a-8d5c-4ccd-b6b2-051d172dd252)


Задание 2
![image](https://github.com/AlexanderSchelokov/Gitlab-08-3/assets/121572590/c49c5a96-e439-430b-9072-5363213c1756)
stages:
  - test
  - build

test:
  stage: test
  image: golang:1.17
  script: 
   - go test .

build:
  stage: build
  image: docker:latest
  script:
   - docker build .
![image](https://github.com/AlexanderSchelokov/Gitlab-08-3/assets/121572590/fa483654-4bd3-4e7f-a4fe-f2fdba3ab7ff)
![image](https://github.com/AlexanderSchelokov/Gitlab-08-3/assets/121572590/5e356795-3c20-4112-81bd-21af1ffff2a8)



