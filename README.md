How to reproduce this bug
--------------------------
 * docker-compose up -d
 * curl -I `http://localhost:8081/čřčžřčž`
 * you get `http://test/?uri=/%C4%8D%C5%99%C4%8D%C5%BE%C5%99%C4%8D%C5%BE&request_uri=/%C4%8D%C5%99%C4%8D%C5%BE%C5%99%C4%8D%C5%BE&test_uri=https://localhost/%C4%8D%C5%99%C4%8D%C5%BE%C5%99%C4%8D%C5%BE`
 
Screenshot
-------------------------
![Nginx Bug](/nginx-redirect-unicode-bug.png?raw=true "Nginx Bug")