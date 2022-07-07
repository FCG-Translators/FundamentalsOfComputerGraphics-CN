# 前言
<br/>
&emsp;&emsp;这一版的《计算机图形学基础》包括对有关纹理和图形硬件等章节的大量重写，并对全书进行了许多更正。现在全书中的图片都是彩色的。  
<br/>
&emsp;&emsp;本书的组织结构与第三版基本相似。根据我们的想法，第2章到第8章成为了“核心的核心（core core）”，通过使用光线追踪和光栅化的互补方法了解图像如何进入屏幕所绝对需要的笔直而狭窄的路径。首先介绍光线追踪，因为它是生成三维场景图像的最简单方法，然后是图形管道所需的数学机制，然后是管道本身。之后，“外部的核心（outer core）”涵盖了通常包含在入门课程中的其他主题，例如采样理论、纹理映射、空间数据结构和样条曲线。从第15章开始是一些被贡献的章节，这些章节由我们选择的具有专业知识和观点表达思路清晰的贡献者撰写。  
<br/>
&emsp;&emsp;在多年来我们对本书进行修订的过程中，我们努力保留了早期版本中非正式的、直观的表述风格，同时也提高了一致性、精确性和完整性。我们希望读者能够发现这本书是一个吸引人的平台，适用于各种计算机图形学课程。  

## 关于封面
<br/>
&emsp;&emsp;封面图片来自 J.W.Baker 《水中之虎》（画布上的拉丝和喷枪亚克力，16英寸×20英寸），www.jwbart.com。  
<br/>
&emsp;&emsp;老虎的主题是指 Alain Fournier（1943-2000）1998年在康奈尔大学的一次研讨会上的精彩演讲。他的谈话是对老虎的动作进行了令人回味的口头描述。他总结了自己的观点：  
<br/>
&emsp;&emsp;尽管在过去的35年里，计算机图形学的建模和渲染已经有了巨大的进展，但我们仍然无法自动模拟在河中游泳的老虎的所有精彩细节。我所说的自动是指不需要艺术家或专家进行仔细的手动调整的方式。  
<br/>
&emsp;&emsp;坏消息是，我们还有很长的路没走。  
<br/>
&emsp;&emsp;好消息是，我们还有很长的路要走。  

## 在线资源
<br/>
&emsp;&emsp;本书的网址是 http://www.cs.cornell.edu/~srm/fcg4/ 。我们将继续维护本书的勘误表和课程链接，以及与本书风格相符的教材。本书中的大多数图片都是 Adobe Illustrator 格式，我们很乐意根据需要将特定图片转换为可移植格式。请随时通过 shirley@cs.utah.edu 或 srm@cs.cornell.edu 与我们联系。  

## 致谢
<br/>
&emsp;&emsp;以下人员提供了本书各版本的有用信息、评论或者反馈：Ahmet O˘guz Aky¨uz, Josh Andersen, Zeferino Andrade, Kavita Bala, Adam Berger, Adeel Bhutta, Solomon Boulos, Stephen Chenney, Michael Coblenz, Greg Coombe, Frederic Cremer, Brian Curtin, Dave Edwards, Jonathon Evans, Karen Feinauer, Amy Gooch, Eungyoung Han, Chuck Hansen, Andy Hanson, Razen Al Harbi, Dave Hart, John Hart, John “Spike” Hughes, Helen Hu, Vicki Interrante, Wenzel Jakob, Doug James, Henrik Wann Jensen, Shi Jin, Mark Johnson, Ray Jones, Revant Kapoor, Kristin Kerr, Erum Arif Khan, Mark Kilgard, Dylan Lacewell, Mathias Lang, Philippe Laval, Marc Levoy, Howard Lo, Joann Luu, Ron Metoyer, Keith Morley, Eric Mortensen, Koji Nakamaru, Micah Neilson, Blake Nelson, Michael Nikelsky, James O’Brien, Steve Parker, Sumanta Pattanaik, Matt Pharr, Peter Poulos, Shaun Ramsey, Rich Riesenfeld, Nate Robins, Nan Schaller, Chris Schryvers, Tom Sederberg, Richard Sharp, Sarah Shirley, Peter-Pike Sloan, Hannah Story, Tony Tahbaz, Jan-Phillip Tiesel, Bruce Walter, Alex Williams, Amy Williams, Chris Wyman, and Kate Zebrose.  
<br/>
&emsp;&emsp;Ching-Kuang Shene 和 David Solomon 允许我们借用他们的例子。 Henrik Wann Jensen、Eric Levin、Matt Pharr 和 Jason Waltman 慷慨地提供了图片。 Brandon Mansfield 帮助改进了关于光线追踪的分层包围体的探讨。 Philip Greenspun (philip.greenspun.com) 热心地允许我们使用他的照片。 John “Spike” Hughes 帮助改进了对抽样理论的探讨。 Wenzel Jakob 的 Mitsuba 渲染器在创建许多图形方面非常宝贵。我们非常感谢 J.W. Baker 帮助创作了 Pete 设想的封面。他除了是一位才华横溢的艺术家之外，也是一位非常愉快的工作伙伴。  
<br/>
&emsp;&emsp;本书的章节注释中引用了许对编写本书有帮助的著作。然而，有几本影响了本书内容和表现形式的关键文献值得在此特别表彰。其中包括两本经典的计算机图形学教材，我们都是从这两本教材中学习的基础知识——《计算机图形学：原理与实践》（Foley、Van Dam、Feiner 和 Hughes，1990 年）和《计算机图形学》（Hearn 和 Baker，1986 年）。其他文本包括 Alan Watt 的两本有影响力的书籍 (Watt, 1993, 1991), Hill的《使用OpenGL的计算机图形》(Francis S. Hill, 2000), Angel的《交互式计算机图形学：使用 OpenGL 的自上而下方法》(Angel, 2002), Hugues Hoppe 的华盛顿大学论文 (Hoppe, 1994) 和 Rogers 的两篇优秀的图形学文章 (D. F. Rogers, 1985, 1989)。  
<br/>
&emsp;&emsp;我们要特别感谢 Alice 和 Klaus Peters 鼓励 Pete 撰写本书的第一版，并感谢他们在完成本书方面的伟大能力。他们对作者的耐心以及竭尽所能奉献于使本书成为最好的书，这对本书的出版起了重要的作用。如果没有他们的非凡努力，这本书肯定不会存在。  
<br/>
<p align="right">盐湖城，犹他州</p>
<p align="right">伊萨卡，纽约</p>
<p align="right">2015年2月</p>  
