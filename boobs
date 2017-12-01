//mux to select the f1 f0 outputs
module mux_4to2(hi_f1, hi_f0, lo_f1, lo_f0, f1, f0);

input hi_f1, hi_f0, lo_f1, lo_f0;
output f1, f0;

//use hi_f1 to select the correct outputs

reg x,y;
always @(hi_f1 or hi_f0 or lo_f1 or lo_f0) begin
	if (hi_f1 == 0)
	    begin
		x = hi_f1;
		y = hi_f0;
	    end
	else
	    begin
		x = lo_f1;
		y = lo_f0;
	    end
end
assign f1 = x;
assign f0 = y;

endmodule

//32-bit tree comparator
module tree_comp(A, B, f1, f0);
input [31 : 0] A, B;
output f1, f0;

wire [31 : 0] f1_L5, f0_L5;
wire [15 : 0] f1_L4, f0_L4;
wire [7 : 0] f1_L3, f0_L3;
wire [3 : 0] f1_L2, f0_L2;
wire [1 : 0] f1_L1, f0_L1;

//write your code here

//Level 5: 32 one_bit_comp go here
	one_bit_comp comp1(A[0], B[0], f1_L5[0], f0_L5[0]);
	one_bit_comp comp2(A[1], B[1], f1_L5[1], f0_L5[1]);
	one_bit_comp comp3(A[2], B[2], f1_L5[2], f0_L5[2]);
	one_bit_comp comp4(A[3], B[3], f1_L5[3], f0_L5[3]);
	one_bit_comp comp5(A[4], B[4], f1_L5[4], f0_L5[4]);
	one_bit_comp comp6(A[5], B[5], f1_L5[5], f0_L5[5]);
	one_bit_comp comp7(A[6], B[6], f1_L5[6], f0_L5[6]);
	one_bit_comp comp8(A[7], B[7], f1_L5[7], f0_L5[7]);
	one_bit_comp comp9(A[8], B[8], f1_L5[8], f0_L5[8]);
	one_bit_comp comp10(A[9], B[9], f1_L5[9], f0_L5[9]);
	one_bit_comp comp11(A[10], B[10], f1_L5[10], f0_L5[10]);
	one_bit_comp comp12(A[11], B[11], f1_L5[11], f0_L5[11]);
	one_bit_comp comp13(A[12], B[12], f1_L5[12], f0_L5[12]);
	one_bit_comp comp14(A[13], B[13], f1_L5[13], f0_L5[13]);
	one_bit_comp comp15(A[14], B[14], f1_L5[14], f0_L5[14]);
	one_bit_comp comp16(A[15], B[15], f1_L5[15], f0_L5[15]);
	one_bit_comp comp17(A[16], B[16], f1_L5[16], f0_L5[16]);
	one_bit_comp comp18(A[17], B[17], f1_L5[17], f0_L5[17]);
	one_bit_comp comp19(A[18], B[18], f1_L5[18], f0_L5[18]);
	one_bit_comp comp20(A[19], B[19], f1_L5[19], f0_L5[19]);
	one_bit_comp comp21(A[20], B[20], f1_L5[20], f0_L5[20]);
	one_bit_comp comp22(A[21], B[21], f1_L5[21], f0_L5[21]);
	one_bit_comp comp23(A[22], B[22], f1_L5[22], f0_L5[22]);
	one_bit_comp comp24(A[23], B[23], f1_L5[23], f0_L5[23]);
	one_bit_comp comp25(A[24], B[24], f1_L5[24], f0_L5[24]);
	one_bit_comp comp26(A[25], B[25], f1_L5[25], f0_L5[25]);
	one_bit_comp comp27(A[26], B[26], f1_L5[26], f0_L5[26]);
	one_bit_comp comp28(A[27], B[27], f1_L5[27], f0_L5[27]);
	one_bit_comp comp29(A[28], B[28], f1_L5[28], f0_L5[28]);
	one_bit_comp comp30(A[29], B[29], f1_L5[29], f0_L5[29]);
	one_bit_comp comp31(A[30], B[30], f1_L5[30], f0_L5[30]);
	one_bit_comp comp32(A[31], B[31], f1_L5[31], f0_L5[31]);

//Level 4: 16 mux_4to2 go here
	mux_4to2 mx41(f1_L5[1], f0_L5[1], f1_L5[0], f0_L5[0], f1_L4[0], f0_L4[0]);
	mux_4to2 mx42(f1_L5[3], f0_L5[3], f1_L5[2], f0_L5[2], f1_L4[1], f0_L4[1]);
	mux_4to2 mx43(f1_L5[5], f0_L5[5], f1_L5[4], f0_L5[4], f1_L4[2], f0_L4[2]);
	mux_4to2 mx44(f1_L5[7], f0_L5[7], f1_L5[6], f0_L5[6], f1_L4[3], f0_L4[3]);
	mux_4to2 mx45(f1_L5[9], f0_L5[9], f1_L5[8], f0_L5[8], f1_L4[4], f0_L4[4]);
	mux_4to2 mx46(f1_L5[11], f0_L5[11], f1_L5[10], f0_L5[10], f1_L4[5], f0_L4[5]);
	mux_4to2 mx47(f1_L5[13], f0_L5[13], f1_L5[12], f0_L5[12], f1_L4[6], f0_L4[6]);
	mux_4to2 mx48(f1_L5[15], f0_L5[15], f1_L5[14], f0_L5[14], f1_L4[7], f0_L4[7]);
	mux_4to2 mx49(f1_L5[17], f0_L5[17], f1_L5[16], f0_L5[16], f1_L4[8], f0_L4[8]);
	mux_4to2 mx410(f1_L5[19], f0_L5[19], f1_L5[18], f0_L5[18], f1_L4[9], f0_L4[9]);
	mux_4to2 mx411(f1_L5[21], f0_L5[21], f1_L5[20], f0_L5[20], f1_L4[10], f0_L4[10]);
	mux_4to2 mx412(f1_L5[23], f0_L5[23], f1_L5[22], f0_L5[22], f1_L4[11], f0_L4[11]);
	mux_4to2 mx413(f1_L5[25], f0_L5[25], f1_L5[24], f0_L5[24], f1_L4[12], f0_L4[12]);
	mux_4to2 mx414(f1_L5[27], f0_L5[27], f1_L5[26], f0_L5[26], f1_L4[13], f0_L4[13]);
	mux_4to2 mx415(f1_L5[29], f0_L5[29], f1_L5[28], f0_L5[28], f1_L4[14], f0_L4[14]);
	mux_4to2 mx416(f1_L5[31], f0_L5[31], f1_L5[30], f0_L5[30], f1_L4[15], f0_L4[15]);

//Level 3: 8 mux_4to2 go here
	mux_4to2 mx31(f1_L4[1], f0_L4[1], f1_L4[0], f0_L4[0], f1_L3[0], f0_L3[0]);
	mux_4to2 mx32(f1_L4[3], f0_L4[3], f1_L4[2], f0_L4[2], f1_L3[1], f0_L3[1]);
	mux_4to2 mx33(f1_L4[5], f0_L4[5], f1_L4[4], f0_L4[4], f1_L3[2], f0_L3[2]);
	mux_4to2 mx34(f1_L4[7], f0_L4[7], f1_L4[6], f0_L4[6], f1_L3[3], f0_L3[3]);
	mux_4to2 mx35(f1_L4[9], f0_L4[9], f1_L4[8], f0_L4[8], f1_L3[4], f0_L3[4]);
	mux_4to2 mx36(f1_L4[11], f0_L4[11], f1_L4[10], f0_L4[10], f1_L3[5], f0_L3[5]);
	mux_4to2 mx37(f1_L4[13], f0_L4[13], f1_L4[12], f0_L4[12], f1_L3[6], f0_L3[6]);
	mux_4to2 mx38(f1_L4[15], f0_L4[15], f1_L4[14], f0_L4[14], f1_L3[7], f0_L3[7]);
//Level 2: 4 mux_4to2 go here
	mux_4to2 mx21(f1_L3[1], f0_L3[1], f1_L3[0], f0_L3[0], f1_L2[0], f0_L2[0]);
	mux_4to2 mx22(f1_L3[3], f0_L3[3], f1_L3[2], f0_L3[2], f1_L2[1], f0_L2[1]);
	mux_4to2 mx23(f1_L3[5], f0_L3[5], f1_L3[4], f0_L3[4], f1_L2[2], f0_L2[2]);
	mux_4to2 mx24(f1_L3[7], f0_L3[7], f1_L3[6], f0_L3[6], f1_L2[3], f0_L2[3]);
//Level 1: 2 mux_4to2 go here
	mux_4to2 mx11(f1_L2[1], f0_L2[1], f1_L2[0], f0_L2[0], f1_L1[0], f0_L1[0]);
	mux_4to2 mx12(f1_L2[3], f0_L2[3], f1_L2[2], f0_L2[2], f1_L1[1], f0_L1[1]);
//Level 0: 1 mux_4to2 goes here
	mux_4to2 mx01(f1_L1[1], f0_L1[1], f1_L1[0], f0_L1[0], f1_L0[0], f0_L0[0]);

endmodule
