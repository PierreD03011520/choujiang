# choujiang
import random

# 定义一个名为 "random_lottery" 的函数
def random_lottery():
    # 定义一个名为 "lottery_numbers" 的列表，其中包含 1 到 50 之间的整数
    lottery_numbers = list(range(1, 51))
    # 使用 random.shuffle() 函数打乱列表中的顺序
    random.shuffle(lottery_numbers)
    # 使用列表推导式从列表中选取前 6 个数字
    winning_numbers = [n for n in lottery_numbers[:6]]
    # 按升序排列
    winning_numbers.sort()
    # 输出中奖号码
    print("Winning numbers: ", winning_numbers)

# 使用函数
random_lottery()
