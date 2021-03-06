# Endpoint

## Current

- URL
  - /current/?key="WEATHERBIT_KEY"
- Method
  - GET
- Parameters
  - key = weatherbit key
- Respone

  ```json
  {
  "data": {
      "current": [
          {
              "aqi": 259,
              "city": "Serang",
              "co": 1842.5,
              "lat": -6.12,
              "lon": 106.15,
              "no2": 19.5354,
              "o3": 85.1154,
              "pm10": 154.762,
              "pm25": 137.529,
              "so2": 5.00679
          },
          {
              "aqi": 162,
              "city": "Bandung",
              "co": 1348.5,
              "lat": -6.92,
              "lon": 107.61,
              "no2": 26.39,
              "o3": 92.9832,
              "pm10": 74.014,
              "pm25": 64.2349,
              "so2": 15.0204
          },
          ...
      ]
    }
  }
  ```

## History & Prediction by latitude longitude

- URL
  - /by_location?lat="LATITUDE"&lon="LONGITUDE"&key="WEATHERBIT_KEY"
- Method
  - GET
- Parameter
  - lat = latitude
  - long = longitude
  - key = weatherbit key
- Response
  ```json
  {
    "data": {
      "forecast": [
        {
          "aqi": 35.63230514526367,
          "co": 250.86363220214844,
          "datetime": "2022-06-10 15:00:00",
          "no2": 1.7819881439208984,
          "o3": 80.52020263671875,
          "pm10": 6.425139904022217,
          "pm25": 4.549275875091553,
          "so2": 0.6959050893783569
        },
        {
          "aqi": 35.75181579589844,
          "co": 253.9100799560547,
          "datetime": "2022-06-10 14:00:00",
          "no2": 1.8818491697311401,
          "o3": 80.3956527709961,
          "pm10": 6.713098049163818,
          "pm25": 4.722179889678955,
          "so2": 0.7107279896736145
        },
        {
          "aqi": 36.89277648925781,
          "co": 260.11260986328125,
          "datetime": "2022-06-10 13:00:00",
          "no2": 1.966313123703003,
          "o3": 79.4944076538086,
          "pm10": 6.969505310058594,
          "pm25": 4.887365341186523,
          "so2": 0.7187684774398804
        }
      ],
      "history": [
        {
          "aqi": 36.0,
          "co": 256.67,
          "datetime": "2022-06-10 12:00:00",
          "no2": 2.8,
          "o3": 78.0,
          "pm10": 6.49,
          "pm25": 4.69,
          "so2": 0.58
        },
        {
          "aqi": 34.0,
          "co": 245.89,
          "datetime": "2022-06-10 11:00:00",
          "no2": 2.39,
          "o3": 74.0,
          "pm10": 5.48,
          "pm25": 4.04,
          "so2": 0.79
        },
        {
          "aqi": 34.0,
          "co": 235.1,
          "datetime": "2022-06-10 10:00:00",
          "no2": 1.99,
          "o3": 72.67,
          "pm10": 4.47,
          "pm25": 3.39,
          "so2": 0.99
        },
        {
          "aqi": 32.0,
          "co": 224.32,
          "datetime": "2022-06-10 09:00:00",
          "no2": 1.58,
          "o3": 70.0,
          "pm10": 3.46,
          "pm25": 2.74,
          "so2": 1.2
        },
        {
          "aqi": 32.0,
          "co": 225.83,
          "datetime": "2022-06-10 08:00:00",
          "no2": 1.46,
          "o3": 70.0,
          "pm10": 3.66,
          "pm25": 2.91,
          "so2": 1.19
        },
        {
          "aqi": 29.0,
          "co": 227.35,
          "datetime": "2022-06-10 07:00:00",
          "no2": 1.34,
          "o3": 63.28,
          "pm10": 3.86,
          "pm25": 3.08,
          "so2": 1.18
        }
      ]
    }
  }
  ```

## History & Prediction by city

- URL
  - /by_city?city="CITY_NAME"&key="WEATHERBIT_KEY"
- Method
  - GET
- Parameter
  - city = city name
  - key = weatherbit key
- Response

```json
{
  "data": {
    "forecast": [
      {
        "aqi": 266.2001953125,
        "co": 6223.35986328125,
        "datetime": "2022-06-10 21:00:00",
        "no2": 77.68670654296875,
        "o3": 111.3797836303711,
        "pm10": 391.13861083984375,
        "pm25": 230.82620239257812,
        "so2": 37.20216369628906
      },
      {
        "aqi": 259.1991882324219,
        "co": 5916.0517578125,
        "datetime": "2022-06-10 20:00:00",
        "no2": 76.00938415527344,
        "o3": 125.09712982177734,
        "pm10": 381.1224060058594,
        "pm25": 196.6309814453125,
        "so2": 36.63417434692383
      },
      {
        "aqi": 269.3083801269531,
        "co": 5821.837890625,
        "datetime": "2022-06-10 19:00:00",
        "no2": 75.07557678222656,
        "o3": 138.59524536132812,
        "pm10": 379.35528564453125,
        "pm25": 192.97633361816406,
        "so2": 36.5171012878418
      }
    ],
    "history": [
      {
        "aqi": 242.0,
        "co": 5463.11,
        "datetime": "2022-06-10 18:00:00",
        "no2": 73.01,
        "o3": 149.91,
        "pm10": 383.14,
        "pm25": 235.92,
        "so2": 34.66
      },
      {
        "aqi": 246.0,
        "co": 4525.27,
        "datetime": "2022-06-10 17:00:00",
        "no2": 58.67,
        "o3": 204.62,
        "pm10": 349.36,
        "pm25": 127.96,
        "so2": 33.96
      },
      {
        "aqi": 181.0,
        "co": 3587.44,
        "datetime": "2022-06-10 16:00:00",
        "no2": 44.34,
        "o3": 259.33,
        "pm10": 315.58,
        "pm25": 20.0,
        "so2": 33.26
      },
      {
        "aqi": 190.0,
        "co": 3780.45,
        "datetime": "2022-06-10 15:00:00",
        "no2": 50.3,
        "o3": 275.02,
        "pm10": 334.14,
        "pm25": 23.0,
        "so2": 34.62
      },
      {
        "aqi": 199.0,
        "co": 3973.46,
        "datetime": "2022-06-10 14:00:00",
        "no2": 56.25,
        "o3": 290.72,
        "pm10": 352.7,
        "pm25": 26.0,
        "so2": 35.98
      },
      {
        "aqi": 225.0,
        "co": 4166.47,
        "datetime": "2022-06-10 13:00:00",
        "no2": 62.21,
        "o3": 306.41,
        "pm10": 371.26,
        "pm25": 16.0,
        "so2": 37.34
      }
    ]
  }
}
```
