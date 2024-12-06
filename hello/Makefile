# Makefile

# 编译器
CC = gcc

# 编译选项
CFLAGS = -Wall -g

# 目标可执行文件名称
TARGET = hello

# 源代码文件
SRCS = hello.c

# 生成的对象文件
OBJS = $(SRCS:.c=.o)

# 默认目标
all: $(TARGET)

# 链接对象文件生成可执行文件
$(TARGET): $(OBJS)
	$(CC) $(CFLAGS) -o $(TARGET) $(OBJS)

# 编译源代码文件生成对象文件
%.o: %.c
	$(CC) $(CFLAGS) -c $< -o $@

# 清理生成的文件
clean:
	rm -f $(TARGET) $(OBJS)

# 伪目标（避免与文件名冲突）
.PHONY: all clean

