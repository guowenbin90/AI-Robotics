# AI-Robotics

## Localization Overview
Belief =Probability  
Sense = product followed by normalization  
Move = Convolution (Addition) 

**Bayes theorem reminder:**  
P(A|B) = P(B|A)*P(A) / P(B)  
 and P(B) = P(B|A)*P(A) + P(B|~A)*P(~A)  
P(A) is prior and P(B|A) is measurement probability  
Theorem of total probability:  
P(B) = Sum P(B/A)*P(A) to normilize the result  

## Kalman Filters

X = estimate  
P = Uncertatinty covariance  
F = State transition matrix  
u = motion vector  
z = measurement  
H = measurement function  
R = measurement noise  
I = identity matrix  
### Measurement update  
y = z - H * x  
S = H * P * H<sup>T</sup> + R   
K = P * H<sup>T</sup> * S<sup>-1</sup>  
x' = x + (K * y)  
P' = (I - k * H) * P
### Prediction
X' = Fx + u  
P' = F * P * F<sup>T</sup> 

## Particle Filters

## Search

## PDI Control

## SLAM
