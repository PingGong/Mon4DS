# Mon4DS

The project SMon4DS (Soundness monitoring for Distributed Stream ) is devoted to ensure the soundness of distributed stream processing (currently for the Storm). Although the Strom already provides a novel message-guaranteeing function, it is still in fact too vague to provide user with engouth information for dignosing in the pratical setting.  

The soundess (reference to the soundess of petri net) here refers to the message, i.e, tuples, are processed consistently w.r.t storm topology (DAG). The issue is by no means trivial, but chanllenging in context of distributed and big stream data. In the pratical setting of Storm, the generated tuples are normall in big magnitude and transmited in various ways among distributed and paralleled processing tasks. These fact pose following issues for tuples processing:
    (1) Big number of tuples 
    (2) Occasionaly tuples Lost
    (3) Casually and wrongly emit tuples 
    (4) Using third-party API with unstable QoS.
    
    
Above issues strongly suggest a real-time and distirbuted monitoring framework for Storm to alert users with enough dignosing information when any unsoundess issues occurred. This is the ambitional goal targetted by The SMon4DS !

