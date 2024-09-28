## API RESTFUL using C++
- In this project i'll use CROW
- With you not using Dev Container, you need to run this command

```bash
apt-get update && apt-get install -y libboost-all-dev libasio-dev git && git clone https://github.com/CrowCpp/Crow.git /opt/Crow && cd /opt/Crow && mkdir build && cd build && cmake .. -DCROW_BUILD_EXAMPLES=OFF -DCROW_BUILD_TESTS=OFF && make
```

- After that compose up your docker-compose 

```bash
   docker-compose up -d
```

- To compile API and run it use:

```bash
   g++ -o api main.cpp -I/opt/Crow/include -L/opt/Crow/build 
-lpthread -std=c++17
```
