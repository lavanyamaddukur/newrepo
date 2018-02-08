# newrepo
demo repository
lavanya here
i am new to github
package com.ford.mss.wdmo.common.business.model;

import org.apache.commons.lang.builder.ToStringBuilder;

import com.ford.it.logging.ILogger;
import com.ford.it.logging.LogFactory;
import com.ford.mss.wdmo.common.util.EqualsUtil;
import com.ford.mss.wdmo.common.util.HashCodeUtil;
import com.ford.mss.wdmo.common.util.StringUtils;
import com.ford.mss.wdmo.wiqs.business.model.Country;
import com.ford.mss.wdmo.wiqs.common.WiqsResourceException;
import com.ford.mss.wdmo.wiqs.common.WiqsRuntimeException;

/**
 * Model Object to Represent Addreess
 * 
 * Note - This object is not directly mapped in Toplink , Model Objects which needs to refer this should Map as a
 * 
 * Aggregate object
 *
 * @author gsanka
 */
public class Address extends BaseBO {
    /**
     * The classname for this class used by logging.
     */
    private static final String CLASS_NAME = Address.class.getName();

    /**
     * The <code>Log</code> instance for this application.
     */
    private static final ILogger log =
            LogFactory.getInstance("JRAS").getLogger(CLASS_NAME);
    
    
    private String  address1;
    
    private String address2;
    
    private String address3;
        
    private String postbox;
    
    private String city;
    
    private  String state;
    
    private  String zipcode;
    
    private  String countryIsoCode;


    


    /**
     * @return Returns the address.
     */
    public String getAddress1() {
        if (this.address1 == null) {
            this.setAddress1("");
        }
        return this.address1;
    }


    /**
     * @return Returns the address2.
     */
    public String getAddress2() {
        if (this.address2 == null) {
            this.setAddress2("");
        }
        return this.address2;
    }


    /**
     * @param address2 The address2 to set.
     */
    public void setAddress2(String address2) {
        this.address2 = address2;
    }


    /**
     * @return Returns the city.
     */
    public String getCity() {
        if (this.city == null) {
           this.setCity("");
        }
        return this.city;
    }


    /**
     * @return Returns the address3.
     */
    public String getAddress3() {
        if (this.address3 == null) {
           this.setAddress3("");
        }
        return this.address3;
    }


