# 外星人入侵小游戏
可随机生成外星飞船


一个使用 Python 和 Pygame 编写的经典外星人入侵游戏。玩家控制一艘飞船，射击不断下降的外星人，随着关卡提升，游戏速度会逐渐加快。

## 功能特性

- **飞船控制**：可以上下左右移动飞船，空格键射击。
- **外星人军团**：多行多列的外星人，左右移动并逐渐下降。
- **计分系统**：每击毁一个外星人获得相应分数。
- **关卡难度**：每消灭一波外星人，下一波移动速度更快。
- **生命限制**：初始拥有 3 条生命，外星人触底或撞到飞船将损失生命。
- **游戏状态**：显示当前得分、最高分、关卡和剩余飞船数量。
- **随机性**：每次单击play按钮后生成的外星人编组都是不一样的
```python
   def _create_alien(self, alien_number, row_number):   
      
       alien = Alien(self)
       alien_width, alien_height = alien.rect.size
       alien.x = alien_width + 2 * alien_width * alien_number
       alien.rect.x = alien.x
       alien.rect.y = alien.rect.height + 2 * alien.rect.height * row_number
       if random.choice([True,False]):
           self.aliens.add(alien)
```




## 安装

### 环境要求
- Python 3.6 或更高版本
- Pygame 库
- 我这里用的编译器是vs2022

### 步骤
1. 克隆本仓库到本地：
   ```bash
   git clone https://github.com/qilin635/alien-invasion.git
   cd alien-invasion
   ```


##如有错误，欢迎提出建议
