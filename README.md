### print("Welcome to my page")

```
from universityofbritishcolumbia import BSc_Computer_Science

class MichaelSheroubi:
  
  def __init__(self, position, requirements):
    self.degree = BSc_Computer_Science(honours=True, gpa=3.9)
    
    self.knowledge = { "language": ('Python', 'Java', 'SQL', 'Cypher'),
                        "theory": ('NLP', 'Graph Theory'),
                        "experience": ('Data Analysis', 'Database Design', 'ETL')}
    
    self.need_to_learn = ['Kubernetes', 'Snowboarding', 'Sowing']
                        
    self.position = position
    self.check_requirements(requirements)
  
  # Check requirements and update need_to_learn
  def check_requirements(self, requirements):
    knowledge = set(x for val in self.knowledge.values())
    for req in requirements:
      if req not in knowledge:
        self.need_to_learn.append(req)
        
      
    
```
