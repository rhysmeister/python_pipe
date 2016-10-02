# python_pipe
A few example python command-line tools showing how to consume piped input and output

ex_output_nums
===============

Output a sequence of ten numbers from the supplied integer or 0 if none is supplied.	

ex_output_nums (Output 0..9)
ex_output_nums 1 (output 1..10)
echo 1 | ex_output_nums (Output 1..10)
ex_output_nums 100 (output 100..109)

ex_sq_num
==========

Output the square of the number supplied.

ex_sq_num 1 (Output 1)
ex_sq_num 100 (Output 10000)
echo 10 | ex_sq_num (Output 100)
echo 8 | ex_sq_num (Output 64)
ex_output_nums | ex_sq_num (Output sq of 0..9)
echo 1 | ex_output_nums | ex_sq_num (Output sq of 1..10)
ex_output_nums 5 | ex_sq_num (Output sq of 5..14)
