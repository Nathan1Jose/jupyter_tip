# jupyter_tip
在jupyter处理数据时的随笔


在data中的三列,V1,V2以及label
绘制散点图
# 对每个标签，绘制V1和V2的散点图，处理之前的数据
for label in labels:
    subset = data[data['label'] == label]
    plt.scatter(subset['V1'], subset['V2'], label=label)

plt.xlabel('V1')
plt.ylabel('V2')
plt.legend()
plt.show()
