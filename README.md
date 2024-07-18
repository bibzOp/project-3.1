# project-3.1
BIT.hdl
CHIP Bit {
    IN in, load;
    OUT out;

    PARTS:
Mux(a=gayout,b=in,sel=load,out=a);
DFF(in=a,out=out,out=gayout);
}
![image](https://github.com/user-attachments/assets/96f63d1a-7704-4004-ad61-8262be85980f)


REGISTER.hdl
 CHIP Register {

    IN  in[16], load;
    OUT out[16];

    BUILTIN Register;
    CLOCKED in, load;
}
![image](https://github.com/user-attachments/assets/4b61473d-4440-46ae-a79f-5fe8e4c3add8)

RAM 8
 CHIP RAM8 {

    IN  in[16], load, address[3];
    OUT out[16];

    BUILTIN RAM8;
    CLOCKED in, load;
}
![image](https://github.com/user-attachments/assets/e1a802dc-9039-4c0e-8af0-171e535b2714)

RAM 64
 CHIP RAM64 {

    IN in[16], load, address[6];
    OUT out[16];

    BUILTIN RAM64;
    CLOCKED in, load;
}
![image](https://github.com/user-attachments/assets/6d97d7c6-6d28-4e0d-a5fe-00c2a22041bf)

