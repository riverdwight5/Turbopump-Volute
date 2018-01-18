# Turbopump-Volute

Inputs, equations, and codes for volute

%variables
throat velocity = C;
flow rate = Q;
throat area = A;
throat section radius = r1;
impeller radius = r2;
distance of throat center from axis = r3;
tongue distance = t;
specific energy = e;
angluar velocity = w;
torque = T;
pumping fluid density = p;
best effeciency point = BEP;
head = H;
gallons per minute = GPM;
revolutions per minute = RPM;
specific speed = N;
shutoff head = h;
max discharge presssure = Pd;
suction head = Ps;
total head pressure = Ph;
max working pressure = P;
design stress = n;
casing factor = f;
volute thickness = Vt;
impeller width = b;
shroud thickness = q;
min entrance width of volute = b2;
angle with radial line of section = phi;
distance between impeller and volute = x;
max entrance width of volute = b3;

%equations
A = (Q*10^6)/C;
r1 = 0.5*sqrt((A*4))/pi);
r3 = r1+r1+t;
BEP = (p*e*Q)/(w*T);
N = (RPM*sqrt(GPM))/H;
Pd = p*h*g;
Ph = Pd+Ps+0.011*Pd;
Vt = (P*r2)/(f*n-0.6*P);
b2 = b+(2*q);
bmax = b2+(2*x*tan(phi/2));
c3 = K*sqrt(2*g*H);
a = (theta*Q)/(3.12*360*c3);
atot = 2*a;
de = di+2*taper*tan(5);
vi = Q/(3.12*Ni);
ve = Q/(3.12*Ne);
rt = 1.05*(0.5*d2);
b4 = 1.75*b;
