# hello-world
Description
Don't know why?
python 1.2.py
cuda:0
Traceback (most recent call last):
  File "1.2.py", line 139, in <module>
    logits = net(g, features)
  File "C:\Users\14044\AppData\Local\Programs\Python\Python37\lib\site-packages\torch\nn\modules\module.py", line 532, in __call__
    result = self.forward(*input, **kwargs)
  File "1.2.py", line 96, in forward
    x = self.gcn2(g, x)
  File "C:\Users\14044\AppData\Local\Programs\Python\Python37\lib\site-packages\torch\nn\modules\module.py", line 532, in __call__
    result = self.forward(*input, **kwargs)
  File "1.2.py", line 84, in forward
    g.apply_nodes(func=self.apply_mod)
  File "C:\Users\14044\AppData\Local\Programs\Python\Python37\lib\site-packages\dgl\graph.py", line 2081, in apply_nodes
    Runtime.run(prog)
  File "C:\Users\14044\AppData\Local\Programs\Python\Python37\lib\site-packages\dgl\runtime\runtime.py", line 11, in run
    exe.run()
  File "C:\Users\14044\AppData\Local\Programs\Python\Python37\lib\site-packages\dgl\runtime\ir\executor.py", line 129, in run
    udf_ret = fn_data(node_data)
  File "C:\Users\14044\AppData\Local\Programs\Python\Python37\lib\site-packages\dgl\runtime\scheduler.py", line 279, in _afunc_wrapper
    return apply_func(nbatch)
  File "C:\Users\14044\AppData\Local\Programs\Python\Python37\lib\site-packages\torch\nn\modules\module.py", line 532, in __call__
    result = self.forward(*input, **kwargs)
  File "1.2.py", line 67, in forward
    self.linear.weight.copy_(self.rnn(node.data['h']))
  File "C:\Users\14044\AppData\Local\Programs\Python\Python37\lib\site-packages\torch\nn\modules\module.py", line 532, in __call__
    result = self.forward(*input, **kwargs)
  File "1.2.py", line 52, in forward
    h_tm1 = cell.forward(x_t, h_tm1)
  File "1.2.py", line 31, in forward
    wx = self.act(h_tm1 * self.u + x_t @ self.w + self.b)
