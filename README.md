# PWM
# Codigo sobre a aula do dia 04/09/2024 com placa arduino 

// C++ code
//
void setup()
{
 Serial.begin(9600);
}

void loop()
{
  for(int digitalInput=0; digitalInput<225; digitalInput++)
  {
    Serial.print("Digital Input:");
    Serial.print(digitalInput);
    analogWrite(11, digitalInput);
    analogWrite(9, digitalInput);
    analogWrite(6, digitalInput);
  }
}
