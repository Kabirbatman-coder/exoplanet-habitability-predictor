Model placement and config

1) Place your converted TFJS files here:
   - public/model/model.json
   - public/model/group1-shard1of1.bin (and any other shard files)

2) Optional mapping/normalization:
   - public/model/feature_map.json
     Example skeleton:
     {
       "features": [
         { "name": "planetRadius", "index": 0, "norm": {"type":"standard","mean":1.0,"std":0.2} },
         { "name": "orbitalPeriod", "index": 1, "norm": {"type":"minmax","min":0,"max":10000} },
         { "name": "stellarMass", "index": 2 },
         { "name": "equilibriumTemp", "index": 3 },
         { "name": "eccentricity", "index": 4 },
         { "name": "stellarRadius", "index": 5 }
         // ... fill remaining indices up to 51 as the model expects 52 features
       ],
       "classLabels": ["non_habitable", "marginal", "prime"]
     }

If feature_map.json is not provided, the app will place the 6 UI fields in indices 0-5 and zero-fill the rest.

3) Enable TFJS inference:
   - Create .env file in project root with:
     REACT_APP_USE_TFJS=true
     # optional override:
     # REACT_APP_TFJS_MODEL_URL=/custom/path/model.json

4) Rebuild and run:
   npm start
   or
   npm run build


