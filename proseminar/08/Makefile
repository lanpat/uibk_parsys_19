CC=gcc
CC_FLAGS=-O0 -g -ggdb -std=c99 -Wall -Wextra -pedantic -lm -fopenmp

.PHONEY: all
all: pi_seq
all: pi_mp
all: matrix_seq
all: matrix_mp
all: matrix_mp_opt
all: heat_stencil_2D_seq
all: heat_stencil_2D_mp
all: heat_stencil_2D_mp_opt


pi_seq: pi_seq.c
	@$(CC) $(CC_FLAGS) $< -o pi_seq

pi_mp: pi_mp.c
	@$(CC) $(CC_FLAGS) $< -o pi_mp

matrix_seq: matrix_seq.c
	@$(CC) $(CC_FLAGS) $< -o matrix_seq

matrix_mp: matrix_mp.c
	@$(CC) $(CC_FLAGS) $< -o matrix_mp

matrix_mp_opt: matrix_mp_opt.c
	@$(CC) $(CC_FLAGS) $< -o matrix_mp_opt

heat_stencil_2D_seq: heat_stencil_2D_seq.c
	@$(CC) $(CC_FLAGS) $< -o heat_stencil_2D_seq

heat_stencil_2D_mp: heat_stencil_2D_mp.c
	@$(CC) $(CC_FLAGS) $< -o heat_stencil_2D_mp

heat_stencil_2D_mp_opt: heat_stencil_2D_mp_opt.c
	@$(CC) $(CC_FLAGS) $< -o heat_stencil_2D_mp_opt





.PHONEY: clean
clean:
	@rm pi_seq
	@rm pi_mp
	@rm matrix_seq
	@rm matrix_mp
	@rm matrix_mp_opt
	@rm heat_stencil_2D_seq
	@rm heat_stencil_2D_mp
	@rm heat_stencil_2D_mp_opt


.PHONEY: run
run: all
	@echo "pi_seq"
	@./pi_seq
	@echo
	@echo "pi_mp"
	@./pi_mp
	@echo
	@echo "matrix_seq"
	@./matrix_seq
	@echo
	@echo "matrix_mp"
	@./matrix_mp
	@echo
	@echo "matrix_mp_opt"
	@./matrix_mp_opt
	@echo
	@echo "heat_stencil_seq"
	@./heat_stencil_2D_seq
	@echo
	@echo "heat_stencil_2D_mp"
	@./heat_stencil_2D_mp
	@echo
	@echo "heat_stencil_2D_mp_opt"
	@./heat_stencil_2D_mp_opt
	@echo
