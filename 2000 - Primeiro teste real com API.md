# Primeiro teste real com API

## Criar conta no OpenWeather API

Acesse: [openweathermap.org](https://openweathermap.org/)

### Crie usuário e senha 
userName: pcfelias65
email: pcfelias65@gmail
password: 4P***YY

### Crie sua API Key
acesse: [API keys](https://home.openweathermap.org/api_keys)

API Key defaut: **456297c2362270b3ecfdb32f8ab7c708**


### Documentação da API Current weather data
acesse: [Current weather data](https://openweathermap.org/current)

### Chamada GET para a previsão do Tempo

[https://api.openweathermap.org/data/2.5/weather?q=Sao%20Paulo,BR&units=metric&lang=pt_br&appid=456297c2362270b3ecfdb32f8ab7c708](https://api.openweathermap.org/data/2.5/weather?q=Sao%20Paulo,BR&units=metric&lang=pt_br&appid=456297c2362270b3ecfdb32f8ab7c708)

### Resposta em JSON

{"coord":{"lon":-46.6361,"lat":-23.5475},"weather":[{"id":701,"main":"Mist","description":"névoa","icon":"50d"}],"base":"stations","main":{"temp":17.84,"feels_like":17.93,"temp_min":17.2,"temp_max":18.38,"pressure":1019,"humidity":86,"sea_level":1019,"grnd_level":928},"visibility":10000,"wind":{"speed":6.17,"deg":170},"clouds":{"all":75},"dt":1757105011,"sys":{"type":1,"id":8394,"country":"BR","sunrise":1757063609,"sunset":1757105838},"timezone":-10800,"id":3448439,"name":"São Paulo","cod":200}

### Resposta Tabulada

| **Informação**       | **Valor**      | **Descrição**                             |
| -------------------- | -------------- | ----------------------------------------- |
| **Cidade**           | São Paulo      | Nome da localidade consultada             |
| **País**             | BR             | Código ISO do país                        |
| **Temperatura**      | 27.3 °C        | Temperatura atual                         |
| **Sensação Térmica** | 28.0 °C        | Como a temperatura é percebida            |
| **Temperatura Mín.** | 26.0 °C        | Menor temperatura do momento              |
| **Temperatura Máx.** | 28.5 °C        | Maior temperatura do momento              |
| **Umidade**          | 55 %           | Umidade relativa do ar                    |
| **Pressão**          | 1015 hPa       | Pressão atmosférica                       |
| **Vento**            | 3.5 m/s (150°) | Velocidade e direção do vento             |
| **Clima**            | Céu limpo      | Descrição do tempo atual                  |
| **Ícone**            | 🌞             | Representação gráfica do clima            |
| **Nascer do Sol**    | 06:40          | Hora aproximada (convertida do timestamp) |
| **Pôr do Sol**       | 18:55          | Hora aproximada (convertida do timestamp) |
| **Latitude**         | -23.5505       | Coordenada da cidade                      |
| **Longitude**        | -46.6333       | Coordenada da cidade                      |


