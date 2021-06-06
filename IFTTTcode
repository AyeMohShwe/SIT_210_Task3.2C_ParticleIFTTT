# SIT_210_Task3.2C_ParticleIFTTT
int data = A0;
int analogValue;
void setup()
{
    pinMode(data, INPUT);
}
void loop()
{
    analogValue = analogRead(data);
    String intensity = String(analogValue);
    if(analogValue > 10)
    {
        Particle.publish("Ambient_Light", "Stops", PRIVATE);
    }
    else
    {
        Particle.publish("Ambient_Light", "Hits", PRIVATE);
    }
    delay(3000);
}
