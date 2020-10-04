# raspAPI
api's

1: Save Sensor value's after every 15 mins
curl --location --request POST 'https://namewhateveryouwant.000webhostapp.com/api/saveSensorValues' \
--header 'Authorization: Bearer 12334567890' \
--form 'values=[{"id": 1, "section": "A", "area": "0", "sensor": "1", "value": "333", "status": 0, "timestamp": "2020-02-17 22:41:23.729463"}, {"id": 2, "section": "A", "area": "0", "sensor": "3", "value": "456", "status": 0, "timestamp": "2020-02-17 22:41:23.729469"}]'

2: Send Pump/Valve Status Conditionally
curl --location --request POST 'https://namewhateveryouwant.000webhostapp.com/api/pumpValveStatus' \
--header 'Authorization: Bearer 12334567890' \
--header 'Content-Type: text/plain' \
--form 'values=[{"pump":"A", "valve":"a", "status":false,"pump_valve_start_request":false,"pump_valve_stop_request":false,"pump_valve_start_request_granted":false,"pump_valve_stop_request_granted":false,"pump_valve_start":false,"pump_valve_stop":true}]'
