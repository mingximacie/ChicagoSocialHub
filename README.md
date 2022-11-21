# ChicagoSocialHub
<h1> This is a full stack web project.</h1>
<p> The main function of this local project is help people who want to know the available status of divvy dockers or bikes 
near some business stores they'd like to go</p>

How to run this program:

Set-Up:

1.Get the API

  Yelp
  
  Google map
  
2.Change the API in Code

  frontend
  
    src -> index.html -> google-map-API
    
    app -> app.module.ts -> google-map-API
    
  backend-build-yelp-reviews
  
    ChicagpSocialHub-Yelp.ipynb -> yelp-API
    
3.Download 

   Node
   
   express
   
  ElasticSearch (I used elasticsearch-7.17.6)
  
  Angular
  
  PostgreSQL
  
  pgAdmin4(PostgreSQL Visualization)
  
  pip install
  
  pip install pprintpp (not in script)
  
  pip install yelpapi(not in script)
  
  Pandas
  
4.Code

  ChicagpSocialHub-Yelp.ipynb
  
    insert locaohost:9200 to elasticsearch
    
  backend-serve.js
  
    Comment line 82,83,435 (content about pg_connection_divvy_trips)
   
5.Run

  a.Run PostgreSQL server
  
  b.ElasticSearch
  
      elasticsearch-7.17.6 -> bin -> elasticsearch
      
  c.backend - node server
  
      go to the dir ChicagoSocialHub_Tutorial_1_Angular_14_Student/backend
      
      terminal/cmd: 
      
         > curl -H "Content-Type: application/json" -XPUT http://localhost:9200/divvy_station_logs/_settings  -d '{"index":{"max_result_window":10000000}}' 
         
        (works on mac, different on windows)
        
         > node server
         
   d.frontend - Angular
   
      go to the dir ChicagoSocialHub_Tutorial_1_Angular_14_Student/frontend
      
      terminal/cmd: 
      
        > ng serve
        
  e.run scripts
  
      ChicagpSocialHub-Yelp.ipynb
      
      Divvy_real-time_status.ipynb
      
  f.run app
  
      Open browser
      
      localhost:4200 
