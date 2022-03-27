#define lighting_sensor 34
#define ecurrent_sensor 32
#define relay_actuator 35

void setup()
{
	pinMode(lighting_sensor, INPUT);
	pinMode(ecurrent_sensor, INPUT);
	pinMode(relay_actuator, OUTPUT);
}

void loop()
{
	float lighting = analogRead(ldr_sensor) * (3.3/4095.0)
	/* float current = analogRead(ecurrent_sensor) * (3.3/4095.0) */
	Serial.println(analogRead(ldr_sensor));
	if(lighting < 2048.0) digitalWrite(relay_actuator, HIGH);
	else digitalWrite(relay_actuator, LOW);

}
