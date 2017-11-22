
main: 
	
	@echo "----預設變數----"
	@echo "----命令行指令----"
	@echo AR 變數 ${AR}
	@echo AS 變數 ${AS}
	@echo CC 變數 ${CC}
	@echo CXX 變數 ${CXX}
	@echo CO 變數 ${CO}
	@echo CPP 變數 ${CPP}
	@echo FC 變數 ${FC}
	@echo GET 變數 ${GET}
	@echo LEX 變數 ${LEX}
	@echo PC 變數 ${PC}
	@echo YACC 變數 ${YACC}
	@echo YACCR 變數 ${YACCR}
	@echo MAKEINFO 變數 ${MAKEINFO}
	@echo TEX 變數 ${TEX}
	@echo TEXI2DVI 變數 ${TEXI2DVI}
	@echo WEAVE 變數 ${WEAVE}
	@echo CWEAVE 變數 ${CWEAVE}
	@echo TANGLE 變數 ${TANGLE}
	@echo CTANGLE 變數 ${CTANGLE}
	@echo RM 變數 ${RM}
	@echo "----命令行參數----"
	@echo ARFLAGS 變數 ${ARFLAGS}
	@echo ASFLAGS 變數 ${ASFLAGS}
	@echo CFLAGS 變數 ${CFLAGS}
	@echo CXXFLAGS 變數 ${CXXFLAGS}
	@echo COFLAGS 變數 ${COFLAGS}
	@echo CPPFLAGS 變數 ${CPPFLAGS}
	@echo FFLAGS 變數 ${FFLAGS}
	@echo GFLAGS 變數 ${GFLAGS}
	@echo LDFLAGS 變數 ${LDFLAGS}
	@echo LFLAGS 變數 ${LFLAGS}
	@echo PFLAGS 變數 ${PFLAGS}
	@echo RFLAGS 變數 ${RFLAGS}
	@echo YFLAGS 變數 ${YFLAGS}
	@echo 
	@echo "$$ make func"
.PHONY: all
all: func main
	@echo "---常數---"
	@echo $?
	@echo all target $^
	@echo first target $<
	@echo this target:$@
	@echo "---over---"
func: 
	@echo "----字串函數----"
	@echo $(subst d,c,abd)
	@echo $(patsubst %.c,%.o,main.c link.c)
	@echo $(strip  a b c )
	@echo $(findstring a,a b c)
	@echo $(filter %.c %.s,a.c b.c f.dll c.s d.s g.o)
	@echo $(filter-out %.c %.s,a.c b.c f.dll c.s d.s g.o)
	@echo $(sort car banana apple)
	@echo $(word 2,foo bar baz)
	@echo $(wordlist 2,3,foo bar baz)
	@echo $(words a b c)
	@echo $(firstword a b c)
	@echo "----文件名函數----"
	@echo $(dir      ./a/ ./ ./a.out )
	@echo $(notdir   ./a/ ./ ./a.out)
	@echo $(suffix   ./a/ ./ ./a.out)
	@echo $(basename ./a/ ./ ./a.out b.out)
	@echo $(addsuffix .out,a b c)
	@echo $(addprefix ./,a b c)
	@echo $(join abc f,de g)
	@echo $(wildcard *)
	@echo "----其他函數----"
	$(foreach var,1 2 3 4,echo  $(var);)
	@echo $(if 1,true, false)
	@echo $(if ,true, false)
	@echo 
	@echo "$$ make all"
nothing:

clean:
	rm -rf *.o