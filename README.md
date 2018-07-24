# Java_EE_Udemy32
Persisting Pilot objects (One To Many Groundwork)

I created PilotService EJB

      @PersistenceContext(unitName = "airline")
	    EntityManager em;
      
      public void addPilot(Pilot p) {
    	em.persist(p);
    }
    
I created AddPilot Servlet

      @EJB
	    PilotService ps;
      
      Pilot p = new Pilot();
		
		  p.setFirstName("Name ");
		  p.setLastName("Last Name");
		  p.setPilotRank(PilotRank.Captain);
		  p.setPilotLicence(random number);
		
		  ps.addPilot(p);


      
