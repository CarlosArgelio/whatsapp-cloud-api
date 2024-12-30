# whatsapp-cloud-api

# Example use

## Import and verified
```py
import WhatsappCloudAPI

whatsapp = WhatsappCloudAPI(token='abc')

# Verified token

whatsapp.verified(secret='abc', mode='', challenge='')
```

## Received message
```py
from WhatsappCloudAPI import ReceivedMessage

received = ReceivedMessage.received(body={})

type_message = ReceivedMessage.type_message
message = ReceivedMessage.message(type_message)
```

## Send Message
```py
from WhatsappCloudAPI import SendMessage

send = SendMessage
send.text_message(to='123', text='Hello World', message_id='123')
send.image(to='123', link='https://image.png', id='123')
```
