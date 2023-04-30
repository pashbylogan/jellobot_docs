## **Shark**`#!py3 class` { #Shark data-toc-label=Shark }



**class methods:** 

 - [`swimclass`](#swimclass)

**class functions & static methods:** 

 - [`be_awesome`](#be_awesome)
 - [`swimstatic`](#swimstatic)

### *Shark*.**swimclass**`#!py3 (a)` { #swimclass data-toc-label=swimclass }

Teach them how to swim

**Parameters**

> **self:** `obj` -- Instance of `Shark`.

**Returns**

> `bool` -- Did they succeed.


??? info "Source Code" 
	```py3 linenums="1 1 2" 
	@classmethod
	def swimclass(self, a):
	    
	    print('prout')
	    print("The shark is swimming.")
	    for i in range(2):
	        print("lololo")
	    return
	
	```
### *Shark*.**be_awesome**`#!py3 (self)` { #be_awesome data-toc-label=be_awesome }

Take the max between two numbers

**Parameters**

> **x:** `float` -- Description of parameter `x`.

> **y:** `float` -- Description of parameter `y`.

**Returns**

> `float` -- Description of returned object.


??? info "Source Code" 
	```py3 linenums="1 1 2" 
	def be_awesome(self):
	    
	    print("The shark is being awesome.")
	
	```
### *Shark*.**swimstatic**`#!py3 (self, a)` { #swimstatic data-toc-label=swimstatic }

Teach them how to swim

**Parameters**

> **self:** `obj` -- Instance of `Shark`.

**Returns**

> `bool` -- Did they succeed.


??? info "Source Code" 
	```py3 linenums="1 1 2" 
	@staticmethod
	def swimstatic(self, a):
	    
	    print('prout')
	    print("The shark is swimming.")
	    for i in range(2):
	        print("lololo")
	    return
	
	```

______

### **maxi**`#!py3 (x: int, y: int = 5)` { #maxi data-toc-label=maxi }

Take the max between two numbers

**Parameters**

> **x:** `float` -- Description of parameter `x`.

> **y:** `float` -- Description of parameter `y`.

**Returns**

> `float` -- Description of returned object.


??? info "Source Code" 
	```py3 linenums="1 1 2" 
	def maxi(x: int, y: int = 5):
	    
	    return np.max(x, y)
	
	```

______

### **maxi2pourvoir**`#!py3 (x, y)` { #maxi2pourvoir data-toc-label=maxi2pourvoir }

Take the max between two numbers

**Parameters**

> **x:** `float` -- Description of parameter `x`.

> **y:** `float` -- Description of parameter `y`.

**Returns**

> `float` -- Description of returned object.


??? info "Source Code" 
	```py3 linenums="1 1 2" 
	def maxi2pourvoir(x, y):
	    
	    return np.max(x, y)
	
	```

______

